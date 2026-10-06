---
title: "IBIT: conciliación del flujo pendiente"
type: report
created: "2026-10-05"
updated: "2026-10-06"
tags: [ibit, bitcoin, etf, provisional]
sources:
  - "../sources/2026-10-05-ibit-conciliacion-flujos-etf.md"
---

# IBIT: conciliación del flujo pendiente

**Corte: 5 de octubre de 2026, 09:35:56, Europe/Madrid.** [Informe completo](../../raw/reports/2026-10-05-ibit-conciliacion-flujos-etf.md) · [Procedencia](../sources/2026-10-05-ibit-conciliacion-flujos-etf.md).

## Estado comprobado

Farside mantiene ausente IBIT del 2 de octubre, tanto en su tabla reciente como en la histórica. El total publicado es 102,7 millones de USD para el 1 de octubre y 31,7 para el 2. El agregado de **134,4 millones sigue siendo provisional**. Se conserva el informe anterior y una [transcripción fechada de todas las columnas de las dos filas](../../raw/data/2026-10-05-farside-etf-1-2-octubre.csv). El guion original no se interpreta como cero.

## Fuente del emisor y cálculo separado

La [exportación original de BlackRock](../../raw/data/2026-10-05-ibit-exportacion-blackrock.xls) muestra NAV y participaciones históricas de [IBIT](../entities/ishares-bitcoin-trust-ibit.md). La [extracción trazable](../../raw/data/2026-10-05-ibit-datos-seleccionados.json) conserva las filas del 30 de septiembre, 1 y 2 de octubre.

Entre el 1 y el 2, las participaciones aumentan en 4.080.000. Multiplicadas por el NAV del 2, 47,637156 USD, producen una **aproximación propia de 194.359.596,48 USD** al valor de emisión neta reflejado por esos saldos.

Ese cálculo no cierra el flujo pendiente: entre el 30 de septiembre y el 1 de octubre la misma fórmula da −9.586.956,60 USD, mientras Farside publica +195,6 millones para IBIT el 1 de octubre. La causa no se ha determinado; fecha de liquidación o convenciones de corte son hipótesis. [Datos, fórmula y límites](../../raw/reports/2026-10-05-ibit-conciliacion-flujos-etf.md).

**No se añade la aproximación al total provisional ni se presenta como flujo publicado de la sesión.** El patrimonio y el volumen negociado tampoco equivalen a flujo neto.

## Cómo cerrar la revisión

Conservar otra captura cuando el dato diario se publique o se concilien fechas y metodología. Recalcular todas las columnas si hay revisiones, indicar proveedor y distinguir cifra publicada de cálculo propio. La wiki debe mantener el valor provisional anterior y su fecha. [Procedimiento completo](../../raw/reports/2026-10-05-ibit-conciliacion-flujos-etf.md).

## Revisión posterior del 6 de octubre

El estado descrito arriba corresponde al corte del día 5 y su RAW permanece intacto. La [captura nueva de Farside](../sources/2026-10-06-farside-flujos-bitcoin.md) ya publica IBIT del 2 y actualiza el agregado del 1–2. Se cierra la ausencia en el proveedor; la diferencia con la aproximación del emisor no queda conciliada. [Informe de la nueva revisión](2026-10-06-seguimiento-ada-night-bitcoin.md).

[Flujos de ETF de Bitcoin](../concepts/flujos-etf-bitcoin.md) · [Bitcoin / BTC](../entities/bitcoin-btc.md) · [Índice de informes](index.md).
