---
title: "Benchmarks locales y rendimiento de una red"
type: concept
created: "2026-10-19"
updated: "2026-10-23"
tags: [benchmarks, metricas, hydra, cardano]
sources:
  - "../sources/2026-10-23-informe-ada-night-bitcoin.md"
  - "../sources/2026-10-21-informe-angry-crypto-show.md"
  - "../sources/2026-10-17-informe-angry-crypto-show.md"
  - "../sources/2026-10-17-cardano-desarrollo-leios-hydra.md"
---

# Benchmarks locales y rendimiento de una red

El caso de [Hydra](../entities/hydra.md) distingue tres magnitudes: **límite de transacciones por snapshot**, **cantidad de operaciones de una ráfaga** y **tiempo de procesamiento en un ensayo concreto**. El [informe semanal ya documentado](../sources/2026-10-17-cardano-desarrollo-leios-hydra.md) y la ampliación del [informe de Angry](../sources/2026-10-17-informe-angry-crypto-show.md) no son mediciones propias de esta wiki.

El ensayo descrito usa **tres nodos locales**, **24.000 autotransferencias mínimas**, **13,50 s frente a 37,04 s**. El límite de snapshot cambia de **1.000 a 4.000**. No se presenta el cociente entre operaciones y segundos como TPS sostenidos de mainnet o una promesa para cualquier aplicación.

Para reutilizar la observación se conservan entorno, número de nodos, tipo de operación, carga y ventana medida, versión si consta y fuente. Una condición que falta no se inventa. Hardware, topología, distribución y condiciones de producción no se han reconstruido en esta ingesta; un ensayo local no mide adopción o demanda de ADA.

[Métricas de uso y adopción](metricas-de-uso-y-adopcion.md) · [Leios, pruebas y mainnet](leios-testnet-y-mainnet.md) · [Versiones y despliegue](versiones-candidatas-y-despliegue.md) · [Índice de conceptos](index.md).

## Comparaciones sin prueba reproducida: Pogun y Leios

El [informe de Angry del 21](../sources/2026-10-21-informe-angry-crypto-show.md) añade dos casos distintos del ensayo local de Hydra. [Pogun](../entities/pogun.md) 1.000x frente a BitVM no identifica métrica, versiones, hardware o carga; no equivale a 1.000x TPS de Cardano. Los 3–5x/10–15x de Leios son objetivos condicionados atribuidos a IOG, sin hilo o medición reproducidos. Se necesita la unidad y condiciones de cada comparación antes de trasladarla a rendimiento de una red.

## Revisión del 23 de octubre

El [nuevo reensayo de Hydra](../sources/2026-10-23-hydra-reensayo-glacier-drop.md) publicado el 22 usa reclamaciones con tres scripts, firmas reales y asignaciones generadas: 24.576 por ejecución, tres por versión en el mismo host. 42 a 79 reclamaciones/s (~1,9x) no se compara directamente con la ráfaga de autotransferencias o el límite por snapshot. Fecha de ejecución no indicada, sin reproducción independiente; no capacidad global o adopción.
