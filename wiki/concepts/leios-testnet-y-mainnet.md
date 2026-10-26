---
title: "Leios: testnet, resultados y mainnet"
type: concept
created: "2026-10-14"
updated: "2026-10-26"
tags: [ada, night, bitcoin, seguimiento]
sources:
  - "../sources/2026-10-24-informe-angry-crypto-show.md"
  - "../sources/2026-10-26-informe-ada-night-bitcoin.md"
  - "../sources/2026-10-23-aviso-angry-acceso-limitado.md"
  - "../sources/2026-10-21-informe-angry-crypto-show.md"
  - "../sources/2026-10-20-informe-angry-crypto-show.md"
  - "../sources/2026-10-17-informe-angry-crypto-show.md"
  - "../sources/2026-10-17-cardano-desarrollo-leios-hydra.md"
  - "../sources/2026-10-15-informe-angry-crypto-show.md"
  - "../sources/2026-10-13-informe-angry-crypto-show.md"
  - "../sources/2026-10-14-cardano-leios-fire.md"
---

# Leios: testnet, resultados y mainnet

## Distinción de estados

[Musashi Dojo en Fire](../sources/2026-10-14-cardano-leios-fire.md) es un entorno de pruebas público: aumentar carga identifica límites, fallos y parámetros. Un objetivo de capacidad o una versión candidata no acredita rendimiento disponible en mainnet. La síntesis evita convertir pruebas de desarrollo en adopción o causas de precio.

La versión candidata puede cambiar formatos y requerir reconstrucción de la testnet. Es una condición del entorno de desarrollo, no una instrucción de mantenimiento para mainnet. No se han ejecutado pruebas propias ni comprobado la decisión final de despliegue.

[Cardano](../entities/cardano-ada.md), [métricas de uso y adopción](metricas-de-uso-y-adopcion.md), [seguimiento](../topics/seguimiento-mercado-ada-night.md), [informe diario](../reports/2026-10-14-seguimiento-ada-night-bitcoin.md).

## Picos citados por el canal

Angry Crypto Show atribuye a mediciones de mercado picos de 329, 436 y 440 TPS en los informes del [8](../sources/2026-10-08-informe-angry-crypto-show.md), [9](../sources/2026-10-09-informe-angry-crypto-show.md) y [13](../sources/2026-10-13-informe-angry-crypto-show.md). No se reproducen esos registros históricos. Un pico de un bloque y una demostración de carga no acreditan rendimiento sostenido de mainnet o despliegue de Leios.

La referencia a Fire del 13 se relaciona con la fuente primaria ya incorporada, manteniendo fecha de anuncio, consulta y entorno. [Métricas y ventanas](metricas-de-uso-y-adopcion.md).

## Objetivo citado en el informe del 15

El [informe de Angry del 15](../sources/2026-10-15-informe-angry-crypto-show.md) atribuye al canal >6.800 actualizaciones y objetivo de hard fork a finales de 2026. El contador no se reprodujo; el contraste previo del autor con la web y roadmap oficial distingue maduración, pruebas y gobernanza. No se transforma el objetivo en fecha garantizada o activación de mainnet. La testnet ya recogida no se cuenta como nuevo anuncio del 15.

## Edición del 17, incorporada el 18 de octubre

El [informe semanal del 16](../sources/2026-10-17-cardano-desarrollo-leios-hydra.md) añade EndorserBlock y consulta del comité. El límite de Hydra de 1.000 a 4.000 transacciones es por snapshot, no una tasa por segundo. No se equiparan componentes en desarrollo, tests locales y capacidad de toda mainnet.

## Ampliación mediada del informe de Angry del 17

El [informe de Angry](../sources/2026-10-17-informe-angry-crypto-show.md) amplía del mismo informe semanal las condiciones del [ensayo de Hydra](benchmarks-locales-y-rendimiento-red.md): tres nodos locales, ráfaga de 24.000 autotransferencias mínimas, 13,50 s frente a 37,04. No es medición propia ni TPS de mainnet. Forecasting y claves BLS son desarrollo; el objetivo de Leios antes de fin de 2026 sigue sin garantizarse y no se aplica automáticamente a Peras.

## Valoración del informe del 20

El [canal atribuye a Hoskinson](../sources/2026-10-20-informe-angry-crypto-show.md) que Leios completaría su visión de Cardano y la califica de escalabilidad infinita. Es una valoración, no benchmark reproducible, capacidad ilimitada demostrada o activación de mainnet. Conserva los estados de desarrollo y las condiciones de pruebas anteriores.

## Multiplicadores atribuidos en el informe del 21

El [canal](../sources/2026-10-21-informe-angry-crypto-show.md) atribuye a IOG 3–5x del throughput actual como inicio y 10–15x sujeto a resultados en mainnet, con aumentos posteriores según demanda y economía de operar la red. El autor enlaza CIP-164 y el sitio técnico para diseño/pruebas, sin cotejar el hilo original o reproducir multiplicadores.

La enumeración de Leios, nested transactions, cuentas, guard scripts, Plutus V4 y recompensas retirables es plan de hard fork, no activación comprobada. El escalado gradual matiza la valoración de «infinito» del episodio anterior, sin convertir ninguna expresión en benchmark o TPS garantizados.

## Discrepancia conservada: revisión completa de Angry del 23

A [según la revisión](../sources/2026-10-23-aviso-angry-acceso-limitado.md) atribuye a Carlos López de Lara hasta **60x** como techo y **10–15x** como primera meta, según demanda/costes. El [informe del 21](../sources/2026-10-21-informe-angry-crypto-show.md) había recogido **3–5x inicial y 10–15x posterior**. Sin declaraciones originales cotejadas o benchmark, se mantienen ambas versiones y sus atribuciones; no se resuelve como cambio oficial, error o rendimiento ya entregado. Tampoco «infinito» se convierte en un dato experimental.

## Revisión del 26 de octubre

[Boletín del 24](../sources/2026-10-26-intersect-dijkstranet-tesoreria.md): DijkstraNet pública en pv11/node 11.1.3; pv12 pendiente. El [informe de desarrollo del 23](../sources/2026-10-26-cardano-desarrollo.md) declara componentes Leios integrados en main del código, no activación mainnet. La fecha interna martes/21 del boletín no se resuelve por inferencia; no se cierran aquí las discrepancias de multiplicadores del canal.

## Angry: edición del 24 completada el 26

El [contraste del autor](../sources/2026-10-24-informe-angry-crypto-show.md) cita CIP-0164 como propuesta y escenarios de 140.000–300.000 bytes de transacciones/s, aproximadamente 100–200 TPS para transacciones medias bajo sus condiciones. No equivalen a cientos de miles de TPS o a una conversión universal. Las cifras del discurso, multiplicadores previos y simulaciones Hydra no se igualan sin versión, carga y entorno comparables; no rendimiento mainnet demostrado.
