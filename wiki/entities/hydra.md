---
title: "Hydra: snapshot y benchmark local"
type: entity
created: "2026-10-19"
updated: "2026-10-23"
tags: [hydra, cardano, escalado]
sources:
  - "../sources/2026-10-23-informe-ada-night-bitcoin.md"
  - "../sources/2026-10-17-informe-angry-crypto-show.md"
  - "../sources/2026-10-17-cardano-desarrollo-leios-hydra.md"
---

# Hydra: snapshot y benchmark local

La [ficha del informe semanal](../sources/2026-10-17-cardano-desarrollo-leios-hydra.md), leída en la preparación de la edición diaria del 17, documenta un límite de **4.000 transacciones por snapshot**, antes 1.000. Es un límite por unidad de snapshot, no una tasa por segundo ni capacidad de toda Cardano.

El [informe de Angry del 17](../sources/2026-10-17-informe-angry-crypto-show.md), preparado el 18, añade del mismo informe semanal un ensayo local de tres nodos con una ráfaga de 24.000 autotransferencias mínimas en 13,50 segundos frente a 37,04. La wiki conserva entorno, carga y origen: no ha ejecutado ese benchmark ni extrapola un promedio de la ráfaga a TPS sostenidos de mainnet.

Las correcciones de reporting, depósitos/fanouts y retiradas en liquidación se atribuyen al informe semanal según la fuente derivada. No se confunden con activación de Leios o Peras. [Benchmarks y entorno](../concepts/benchmarks-locales-y-rendimiento-red.md) · [Leios](../concepts/leios-testnet-y-mainnet.md) · [Cardano](cardano-ada.md) · [Índice de entidades](index.md).

## Revisión del 23 de octubre

El [reensayo publicado el 22](../sources/2026-10-23-hydra-reensayo-glacier-drop.md) compara 0.22.4 y Hydra actual sobre 24.576 reclamaciones: tres ejecuciones por versión en la misma máquina, 42 frente a 79 reclamaciones/s (~1,9x). Es otro entorno y carga que las autotransferencias del ensayo previo; no cifras contradictorias ni rendimiento de toda mainnet. El equipo operativo firma el resultado; no reproducido independientemente. El reparto de NIGHT es histórico de 2025.
