---
title: "Midnight: fundamentos científicos frente a implementación documentada"
type: report
created: "2026-10-05"
updated: "2026-10-05"
tags: [midnight, implementacion, investigacion]
capture_timezone: "Europe/Madrid"
cutoff: "2026-10-05T09:35:56+02:00"
author: "Codex, informe elaborado a petición del usuario"
status: "contraste parcial documentado"
---

# Midnight: fundamentos científicos frente a implementación documentada

## Pregunta y resultado

¿Cómo corresponden los cinco fundamentos científicos seleccionados con el código y los parámetros actuales de Midnight?

Se comprueban mecanismos concretos relacionados con Kachina, generación de DUST, interoperabilidad con Cardano y valoración de recursos. **No hay equivalencia completa demostrada entre los cinco artículos y el protocolo desplegado.** El consenso del nodo revisado usa AURA y GRANDPA; no corresponde a la combinación PoW/PoS de Minotaur. Esta conclusión se refiere a una revisión fija del código y a la versión recomendada por la documentación, no a una auditoría de mainnet.

Informe creado y capturado el 5 de octubre de 2026, con corte de investigación a las 09:35:56 de Madrid. Las publicaciones académicas son anteriores; sus fechas y versiones están en la [bibliografía archivada](../articles/2026-10-05-midnight-bibliografia.md).

## Versiones y alcance del contraste

Las [notas oficiales del nodo](https://docs.midnight.network/relnotes/node), actualizadas el 2 de octubre, mantienen el encabezado 1.0.2 pero indican que ha sido sustituido y que en Preview, Preprod y Mainnet debe utilizarse node/toolkit 1.0.300. No se deduce la versión vigente solo de ese encabezado.

Se resolvió la etiqueta node-1.0.300 a la revisión `c3895bd2bd930b03ad53a4c8de0d98a490b8bfcb`; su [Cargo.toml](../repos/2026-10-05-midnight-implementacion/node/Cargo.toml) fija midnight-ledger 8.1.2. La etiqueta ledger-8.1.2 se resolvió a `36d7442172136758e33009f75ff4aa56616cff40`. El commit del tag del nodo difiere del target de la ficha de release reemitida; se conserva esa diferencia en el [manifiesto](../repos/2026-10-05-midnight-implementacion/manifiesto.json). Las ramas de desarrollo y los candidatos de ledger 9 no se usan como prueba de despliegue.

## Correspondencia por trabajo

| Trabajo | Evidencia examinada | Conclusión y límite |
|---|---|---|
| [Kachina](../articles/2026-10-05-kachina-foundations-private-smart-contracts.pdf), resumen e introducción, PDF pp. 2–3 | La [documentación Kachina](https://docs.midnight.network/concepts/kachina) relaciona estado público, privado y pruebas. La [especificación de contratos](../repos/2026-10-05-midnight-implementacion/ledger/spec/contracts.md) define transcripciones y comprobaciones del contrato; el [código de estructuras](../repos/2026-10-05-midnight-implementacion/ledger/ledger/src/structure.rs) importa transcripciones y tipos de prueba. | Correspondencia arquitectónica concreta. Las transcripciones garantizada y falible son detalles de esta implementación. No se ha demostrado una correspondencia formal completa con el teorema de seguridad UC del artículo. |
| [Blockchain Space Tokenization](../articles/2026-10-05-blockchain-space-tokenization.pdf), resumen e introducción, PDF pp. 1–3 | El [módulo DUST](../repos/2026-10-05-midnight-implementacion/ledger/ledger/src/dust.rs) contiene generación respaldada por NIGHT, capacidad, degradación y registro. La [documentación BST](https://docs.midnight.network/concepts/blockchain-space-tokenization) atribuye a Midnight la incorporación de varias ideas centrales. | Adaptación reconocible del vínculo entre tenencia y capacidad de uso. No se verificaron una política de mempool equivalente a la del artículo ni sus garantías de demora bajo sus supuestos. No debe afirmarse que cualquier transacción tiene un plazo de inclusión garantizado. |
| [Minotaur](../articles/2026-10-05-minotaur-multi-resource-blockchain-consensus.pdf), resumen e introducción, PDF pp. 1–2 | El [README del nodo](../repos/2026-10-05-midnight-implementacion/node/README.md), sección Consensus, declara AURA para producción, GRANDPA para finalidad y BEEFY para soporte de puentes. [service.rs](../repos/2026-10-05-midnight-implementacion/node/node/src/service.rs) arranca esos componentes. | **No coincide con el consenso PoW/PoS de Minotaur.** La inclusión del artículo en el recorrido de investigación de IOG no demuestra su implantación literal. No se trasladan sus garantías de fungibilidad de recursos al nodo revisado. |
| [Proof-of-Stake Sidechains](../articles/2026-10-05-proof-of-stake-sidechains.pdf), resumen e introducción, PDF pp. 2–4 | El [runtime](../repos/2026-10-05-midnight-implementacion/node/runtime/src/lib.rs), líneas 541–563, integra selección de autoridades con un parámetro que distingue candidatos autorizados y registrados. [Ariadne](../repos/2026-10-05-midnight-implementacion/node/partner-chains/toolkit/committee-selection/selection/src/ariadne.rs) incluye selección ponderada, y [cNIGHT observation](../repos/2026-10-05-midnight-implementacion/node/pallets/cnight-observation/src/lib.rs) procesa información de Cardano. | Relación concreta con partner chains y observación de la cadena principal. La [documentación oficial](https://docs.midnight.network/concepts/sidechains-partnerchains) atribuye aislamiento de fallos al diseño; eso no sustituye una prueba del puente actual. La composición real del comité y sus parámetros en mainnet no fueron consultados. |
| [Precios unidimensionales y multidimensionales](../articles/2026-10-05-one-dimensional-vs-multi-dimensional-pricing.pdf), resumen y resultados, PDF pp. 1–3 | [cost_model.rs](../repos/2026-10-05-midnight-implementacion/ledger/base-crypto/src/cost_model.rs), líneas 289–400, distingue factores de lectura, cómputo, tamaño y escritura; los ajusta por ocupación, aplica un suelo relativo y normaliza. [semantics.rs](../repos/2026-10-05-midnight-implementacion/ledger/ledger/src/semantics.rs), líneas 1438–1473, actualiza los precios tras el bloque; la [API del nodo](../repos/2026-10-05-midnight-implementacion/node/ledger/src/versions/common/api/ledger.rs), líneas 187–205, pasa la ocupación al ledger. | Hay un mecanismo multidimensional implementado que termina en una tarifa en DUST. No es una reproducción acreditada de todos los esquemas del artículo: la fórmula usa un máximo entre ciertos costes, suma escritura y churn, y ajusta factores con restricciones. No se ha evaluado su bienestar, convergencia o comportamiento real bajo congestión. |

Los enlaces de código conservan copias locales. También pueden comprobarse en GitHub: [nodo fijado](https://github.com/midnightntwrk/midnight-node/blob/c3895bd2bd930b03ad53a4c8de0d98a490b8bfcb/README.md), [contratos](https://github.com/midnightntwrk/midnight-ledger/blob/36d7442172136758e33009f75ff4aa56616cff40/spec/contracts.md), [precios](https://github.com/midnightntwrk/midnight-ledger/blob/36d7442172136758e33009f75ff4aa56616cff40/base-crypto/src/cost_model.rs) y [actualización tras bloque](https://github.com/midnightntwrk/midnight-ledger/blob/36d7442172136758e33009f75ff4aa56616cff40/ledger/src/semantics.rs). El vínculo histórico de los cinco trabajos es una [atribución de IOG publicada el 6 de marzo de 2026](https://www.iog.io/news/from-research-to-reality-building-midnight-on-peer-reviewed-foundations).

## Parámetros: código inicial frente a estado vigente

En [structure.rs](../repos/2026-10-05-midnight-implementacion/ledger/ledger/src/structure.rs), líneas 2999–3001, se definen 24.000 millones de NIGHT como máximo, 1.000.000 de STAR por NIGHT y 1.000.000.000.000.000 de SPECK por DUST.

En [dust.rs](../repos/2026-10-05-midnight-implementacion/ledger/ledger/src/dust.rs), líneas 1300–1304, los valores **iniciales** son capacidad de 5 DUST por NIGHT, tasa de generación/degradación 8.267 en las unidades del algoritmo y periodo de gracia de tres horas. El comentario describe aproximadamente una semana para llegar al tope. No equivalen a una lectura de parámetros vigentes en mainnet.

Existe una discrepancia verificable: la [especificación de costes](../repos/2026-10-05-midnight-implementacion/ledger/spec/cost-model.md), líneas 153–160, propone 20.000 bytes escritos por bloque, mientras [INITIAL_LIMITS del código](../repos/2026-10-05-midnight-implementacion/ledger/ledger/src/structure.rs), líneas 1173–1184, establece 50.000. Se conservan ambas versiones; para el valor inicial de esta revisión se prioriza el código. No se atribuye ninguna de las dos al estado vivo sin lectura en cadena.

## Incertidumbres y próximos contrastes

- Confirmar runtime, parámetros de ledger y composición del comité en un bloque finalizado de Mainnet, guardando hash, altura, hora y proveedor.
- Comparar el código del puente y las hipótesis de seguridad con la construcción concreta del artículo de sidechains.
- Verificar las condiciones del mempool y ensayar congestión antes de trasladar garantías de BST.
- Relacionar circuitos, compilador y runtime con la formalización de Kachina; este examen documental no certifica su implementación criptográfica.
- Medir precios y uso bajo carga para contrastar los resultados económicos del artículo de precios.

La [referencia de entornos](https://docs.midnight.network/relnotes/network) indica que el acceso público Mainnet ha migrado a Blockfrost y exige un token de proyecto. En este informe no se utilizaron credenciales ni se consultó Mainnet. No se infiere precio ni rentabilidad de NIGHT.

