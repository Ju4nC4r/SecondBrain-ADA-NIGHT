---
title: "Midnight: investigación e implementación, correspondencia por mecanismo"
type: comparison
created: "2026-10-05"
updated: "2026-10-05"
tags: [midnight, comparacion, codigo]
sources:
  - "../sources/2026-10-05-midnight-fundamentos-implementacion.md"
---

# Midnight: investigación e implementación

Comparación reutilizable basada en el [informe de contraste](../reports/2026-10-05-midnight-fundamentos-implementacion.md), con corte el 5 de octubre de 2026 a las 09:35:56 de Madrid. Los [metadatos](../../raw/repos/2026-10-05-midnight-implementacion/manifiesto.json) fijan nodo 1.0.300 y ledger 8.1.2; no se consultó el estado de mainnet.

| Trabajo | Localización de la evidencia | Interpretación |
|---|---|---|
| [Kachina](../sources/kachina-foundations-private-smart-contracts.md) | [Especificación de contratos](../../raw/repos/2026-10-05-midnight-implementacion/ledger/spec/contracts.md), transcripciones garantizadas/falibles; [estructuras](../../raw/repos/2026-10-05-midnight-implementacion/ledger/ledger/src/structure.rs). | Correspondencia arquitectónica. No prueba formal completa de implementación. |
| [BST](../sources/blockchain-space-tokenization.md) | [DUST](../../raw/repos/2026-10-05-midnight-implementacion/ledger/ledger/src/dust.rs), INITIAL_DUST_PARAMETERS, líneas 1300–1304. | Capacidad generada por NIGHT; garantías de espera y mempool no contrastadas. |
| [Minotaur](../sources/minotaur-multi-resource-blockchain-consensus.md) | [README del nodo](../../raw/repos/2026-10-05-midnight-implementacion/node/README.md), líneas 111–113; [servicio](../../raw/repos/2026-10-05-midnight-implementacion/node/node/src/service.rs), arranque de AURA y GRANDPA. | Diferencia concreta: no corresponde a la combinación PoW/PoS del artículo. |
| [Proof-of-Stake Sidechains](../sources/proof-of-stake-sidechains.md) | [Runtime](../../raw/repos/2026-10-05-midnight-implementacion/node/runtime/src/lib.rs), líneas 541–563; [Ariadne](../../raw/repos/2026-10-05-midnight-implementacion/node/partner-chains/toolkit/committee-selection/selection/src/ariadne.rs); [observación cNIGHT](../../raw/repos/2026-10-05-midnight-implementacion/node/pallets/cnight-observation/src/lib.rs). | Hay mecanismos de partner chains. Se desconoce aquí la mezcla real de candidatos autorizados/registrados en mainnet y no se ha demostrado la seguridad completa del puente. |
| [Precios multidimensionales](../sources/one-dimensional-vs-multi-dimensional-pricing.md) | [Modelo de costes](../../raw/repos/2026-10-05-midnight-implementacion/ledger/base-crypto/src/cost_model.rs), líneas 289–400; [semántica](../../raw/repos/2026-10-05-midnight-implementacion/ledger/ledger/src/semantics.rs), líneas 1438–1473; [API del nodo](../../raw/repos/2026-10-05-midnight-implementacion/node/ledger/src/versions/common/api/ledger.rs), líneas 187–205. | Precios por dimensión implementados, con suelo relativo y normalización; cobro final en DUST. No se demuestra equivalencia económica completa con los modelos del artículo. |

Los nombres AURA, GRANDPA y BEEFY se refieren a componentes distintos de producción, finalidad y soporte de puentes. La participación en la selección de autoridades no convierte ese consenso en Minotaur.

La divergencia entre 20.000 bytes escritos propuestos en la especificación y 50.000 en el código inicial está documentada en el [informe](../reports/2026-10-05-midnight-fundamentos-implementacion.md). Los parámetros iniciales no son una lectura de parámetros vivos.

[Midnight, NIGHT y DUST](../entities/midnight-night-dust.md) · [Modelo token-recurso](../concepts/modelo-token-recurso.md) · [Índice de comparaciones](index.md).

