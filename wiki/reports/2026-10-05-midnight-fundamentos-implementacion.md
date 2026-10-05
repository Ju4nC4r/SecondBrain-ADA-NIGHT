---
title: "Midnight: fundamentos científicos frente a implementación"
type: report
created: "2026-10-05"
updated: "2026-10-05"
tags: [midnight, investigacion, implementacion]
sources:
  - "../sources/2026-10-05-midnight-fundamentos-implementacion.md"
---

# Midnight: fundamentos científicos frente a implementación

**Corte: 5 de octubre de 2026, 09:35:56, Europe/Madrid.** [Informe completo en RAW](../../raw/reports/2026-10-05-midnight-fundamentos-implementacion.md) y [procedencia de la fuente](../sources/2026-10-05-midnight-fundamentos-implementacion.md).

## Conclusión

Hay correspondencia comprobable entre mecanismos del código y varios fundamentos científicos. No se ha demostrado equivalencia completa con los cinco artículos ni con el estado desplegado. **Minotaur no describe el consenso del nodo revisado:** el README y el arranque del servicio muestran AURA, GRANDPA y BEEFY.

Se usó node-1.0.300, recomendado por las notas oficiales para mainnet, con su revisión resuelta del tag; Cargo.toml fija ledger 8.1.2. Las revisiones y los originales están en el [manifiesto de captura](../../raw/repos/2026-10-05-midnight-implementacion/manifiesto.json). El target de la ficha de release reemitida difiere del commit del tag; la comparación utiliza el segundo. Las ramas de desarrollo no prueban un despliegue.

## Qué corresponde y qué falta

| Fundamento | Correspondencia comprobada | Garantía o equivalencia pendiente |
|---|---|---|
| [Kachina](../sources/kachina-foundations-private-smart-contracts.md) | Estado público/privado, transcripciones y pruebas en la documentación y estructura del ledger. | Correspondencia formal completa con el modelo y teorema UC. |
| [BST](../sources/blockchain-space-tokenization.md) | DUST respaldado por NIGHT, generación, tope y degradación en el código. | Política de mempool y plazos de inclusión equivalentes al artículo. |
| [Minotaur](../sources/minotaur-multi-resource-blockchain-consensus.md) | Relación histórica atribuida por IOG. | El nodo revisado no usa su combinación PoW/PoS; no se trasladan sus garantías. |
| [Sidechains](../sources/proof-of-stake-sidechains.md) | Selección de autoridades, datos de Cardano y mecanismos de partner chains. | Composición real del comité, prueba del puente y propiedad de aislamiento para esta implementación. |
| [Precios multidimensionales](../sources/one-dimensional-vs-multi-dimensional-pricing.md) | Factores por recurso y ajuste tras cada bloque, conectados a la API del nodo. | Equivalencia con todos los modelos del artículo y resultados económicos bajo carga real. |

La [comparación detallada](../comparisons/midnight-investigacion-e-implementacion.md) enlaza los archivos y líneas relevantes. Estos son resultados de inspección documental y de código, no de ejecución o auditoría criptográfica.

## Parámetros y diferencia documentada

Los valores iniciales de la revisión ledger 8.1.2 son 5 DUST de capacidad por NIGHT, tasa 8.267 en las unidades del algoritmo, aproximadamente una semana hasta el tope según el comentario y tres horas de gracia. Las unidades atómicas son un millón de STAR por NIGHT y mil billones de SPECK por DUST; el máximo definido de NIGHT es 24.000 millones. Véanse [dust.rs, INITIAL_DUST_PARAMETERS](../../raw/repos/2026-10-05-midnight-implementacion/ledger/ledger/src/dust.rs) y [structure.rs](../../raw/repos/2026-10-05-midnight-implementacion/ledger/ledger/src/structure.rs).

**Discrepancia conservada:** la especificación propone 20.000 bytes escritos por bloque; INITIAL_LIMITS del código establece 50.000. Se prioriza el código para el valor inicial de esta revisión, sin atribuirlo al estado vigente de la red. [Especificación](../../raw/repos/2026-10-05-midnight-implementacion/ledger/spec/cost-model.md) y [código](../../raw/repos/2026-10-05-midnight-implementacion/ledger/ledger/src/structure.rs).

## Investigación restante

Falta leer un bloque finalizado de mainnet con runtime, parámetros y autoridades, estudiar la seguridad del puente, contrastar mempool y medir funcionamiento bajo congestión. El acceso público Mainnet documentado exige un token de Blockfrost; no se hizo una consulta autenticada. Esta limitación está registrada en la [fuente archivada](../sources/2026-10-05-midnight-fundamentos-implementacion.md).

[Midnight / NIGHT](../entities/midnight-night.md) · [Fundamentos científicos](../topics/midnight-fundamentos-cientificos.md) · [Índice de informes](index.md).

