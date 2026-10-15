---
title: "Flujos de ETF al contado de Bitcoin"
type: concept
created: "2026-10-05"
updated: "2026-10-14"
tags: [bitcoin, etf, mercado]
sources:
  - "../sources/2026-10-14-farside-flujos-bitcoin.md"
  - "../sources/2026-10-13-farside-flujos-bitcoin.md"
  - "../sources/2026-10-09-farside-flujos-bitcoin.md"
  - "../sources/2026-10-08-farside-flujos-bitcoin.md"
  - "../sources/2026-10-07-farside-flujos-bitcoin.md"
  - "../sources/2026-10-05-informe-ada-night-bitcoin.md"
  - "../sources/2026-10-06-farside-flujos-bitcoin.md"
---

# Flujos de ETF al contado de Bitcoin

## Uso documentado

El informe del 5 de octubre usa las entradas netas en ETF al contado estadounidenses de Bitcoin como contexto de demanda a través de fondos. No detalla la metodología de cálculo ni la estructura de los productos. [Informe archivado](../../raw/reports/2026-10-05-informe-ada-night-bitcoin.md).

## Ejemplo histórico atribuido

Para las sesiones del 1 y 2 de octubre de 2026, el documento recoge 102,7 y 31,7 millones de dólares, respectivamente, con un agregado de 134,4 millones. Indica que el dato de IBIT del día 2 estaba pendiente, por lo que el agregado es **provisional**. La noticia se publicó, según el informe, el 4 de octubre. [Fuente y fechas](../sources/2026-10-05-informe-ada-night-bitcoin.md).

## Interpretación y límites

La fuente señala que estos flujos no garantizan continuidad de la demanda ni explican por sí solos el movimiento de precio del día. Para comparar sesiones deben conservarse las versiones, proveedor, unidad, fechas de sesión y captura, cobertura y estado de revisión. Una celda ausente no equivale a cero.

## Revisión del 5 de octubre

La [conciliación incorporada](../reports/2026-10-05-ibit-conciliacion-flujos-etf.md), con corte a las 09:35:56 de Madrid, conserva las dos filas observadas de Farside y la exportación original del emisor de [IBIT](../entities/ishares-bitcoin-trust-ibit.md). El dato de IBIT del 2 de octubre sigue ausente; 134,4 millones continúa siendo provisional.

Una aproximación propia basada en NAV y variación de participaciones da unos 194,4 millones, pero la misma fórmula discrepa con Farside para la sesión anterior. No se suma al agregado ni se presenta como flujo definitivo. Fecha de liquidación o convenciones de corte siguen siendo hipótesis pendientes. [Fuente, datos y fórmula](../sources/2026-10-05-ibit-conciliacion-flujos-etf.md).

## Revisión del 6 de octubre

La [captura posterior](../sources/2026-10-06-farside-flujos-bitcoin.md) ya contiene IBIT del 2; el agregado del 1–2 pasa de 134,4 provisionales a 292,6 millones de USD publicados. Se conservan las doce columnas y el total de cada sesión, sin modificar el archivo anterior. La diferencia con el cálculo del emisor sigue sin explicar y los datos del proveedor pueden revisarse.

## Revisión del 7 de octubre

La [nueva fila del proveedor](../sources/2026-10-07-farside-flujos-bitcoin.md), para la sesión del 6, contiene doce fondos y total +118,8 millones de USD. Se comprueba la suma de columnas y se archiva un CSV nuevo. Las versiones anteriores permanecen intactas; todas las celdas de esta fila están presentes, pero los datos siguen siendo revisables. [Informe del 7](../reports/2026-10-07-seguimiento-ada-night-bitcoin.md).

## Revisión del 8 de octubre

La [fila de la sesión del 7](../sources/2026-10-08-farside-flujos-bitcoin.md) muestra total −484,9 millones de USD y doce columnas presentes. La suma se comprueba y la versión se archiva en un CSV nuevo. No confundir flujos netos de fondos con ventas simultáneas de BTC; tampoco inferir una tendencia sostenida de una sesión. [Informe del 8](../reports/2026-10-08-seguimiento-ada-night-bitcoin.md).

## Revisión del 9 de octubre

La [fila del 8](../sources/2026-10-09-farside-flujos-bitcoin.md) contiene doce cifras, suma −244,1 millones USD comprobada. Junto con el 7, −729,0 por cálculo propio. Fila completa no equivale a conciliación por emisor. Los flujos miden exposición neta de los fondos y no son el agregado de [liquidaciones de derivados](liquidaciones-posiciones-apalancadas.md); no se suman esas medidas ni se infiere una causa de precio por coincidencia temporal.

## Revisión del 13 de octubre

[Sesión del12](../sources/2026-10-13-farside-flujos-bitcoin.md):-65,4 millonesUSD,total igual aIBIT; doce cifras presentes,suma verificada. Una fila completa sigue siendo revisable y no equivale a conciliación de emisores ni ventas simultáneas deBTC.

## Revisión del 14 de octubre

La [sesión del 13](../sources/2026-10-14-farside-flujos-bitcoin.md) contiene doce cifras y suma +175,7 millones de USD. Se distingue de las [compras de Strive](../sources/2026-10-14-strive-compras-bitcoin.md): compras del 5–9, anuncio del 13; no son la misma ventana ni una medida sumable automáticamente.

## Relaciones

- [Informe del 6 de octubre](../reports/2026-10-06-seguimiento-ada-night-bitcoin.md).
- [Bitcoin / BTC](../entities/bitcoin-btc.md).
- [Informe del 5 de octubre](../reports/2026-10-05-seguimiento-ada-night-bitcoin.md).
- [Seguimiento de mercado](../topics/seguimiento-mercado-ada-night.md).
