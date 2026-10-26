---
title: "Flujos de ETF al contado de Bitcoin"
type: concept
created: "2026-10-05"
updated: "2026-10-26"
tags: [bitcoin, etf, mercado]
sources:
  - "../sources/2026-10-26-informe-ada-night-bitcoin.md"
  - "../sources/2026-10-23-informe-ada-night-bitcoin.md"
  - "../sources/2026-10-19-informe-ada-night-bitcoin.md"
  - "../sources/2026-10-17-farside-flujos-bitcoin.md"
  - "../sources/2026-10-16-farside-flujos-bitcoin.md"
  - "../sources/2026-10-15-informe-ada-night-bitcoin.md"
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

## Revisión del 15 de octubre

La [nota del informe del 15](../sources/2026-10-15-informe-ada-night-bitcoin.md) conserva la sesión del 14: IBIT −110,9, FBTC −152,7, BITB +2,2 y nueve fondos a cero, en millones de USD. Suma recalculada **−261,4**, doce valores presentes. Es una comprobación aritmética del archivo, sin nueva consulta del proveedor ni conciliación por emisor; publicación sin hora y datos revisables. Las compras de Strive del 12–13 corresponden a otra ventana y no se suman como demanda simultánea.

## Relaciones

- [Informe del 6 de octubre](../reports/2026-10-06-seguimiento-ada-night-bitcoin.md).
- [Bitcoin / BTC](../entities/bitcoin-btc.md).
- [Informe del 5 de octubre](../reports/2026-10-05-seguimiento-ada-night-bitcoin.md).
- [Seguimiento de mercado](../topics/seguimiento-mercado-ada-night.md).

## Revisión del 16 de octubre

La [sesión del 15](../sources/2026-10-16-farside-flujos-bitcoin.md) suma +5,1 millones USD: IBIT +16,8, BTCO −4,1, BTC de Grayscale −7,6, otros nueve 0,0. Doce celdas presentes; dato completo no significa definitivo. La sesión previa negativa se mantiene como historia, sin sobrescribirla. No explica por sí sola el rebote descrito por el medio.

## Edición del 17, incorporada el 18 de octubre

La [fila del 16](../sources/2026-10-17-farside-flujos-bitcoin.md), leída el 18, suma −82,4 millones USD: IBIT −71,8 y FBTC −10,6. Otras diez cifras presentes a cero. Se preserva el saldo de la sesión anterior como otro periodo; el cambio de signo no es una contradicción ni causa comprobada de precio.

## Revisión del 19 de octubre

En la [consulta del 19](../sources/2026-10-19-informe-ada-night-bitcoin.md) no hay fila de sesión del 19. La ausencia se conserva como estado de publicación, no un flujo cero. Los datos del 16 permanecen históricos en su ficha, sin presentarlos otra vez como nuevos.

## Revisión del 20 de octubre

La [fila del 19, consultada el 20](../sources/2026-10-20-farside-flujos-bitcoin.md), suma +526,7 millones USD: IBIT +665,2, FBTC −83,6, GBTC −54,9 y nueve fondos a cero. Doce cifras presentes y suma comprobada. La [consulta del 19](../sources/2026-10-19-informe-ada-night-bitcoin.md) no contenía esa fila; se conserva como fotografía anterior. No se suma a compras corporativas del 12–18 ni prueba causalidad de precio.

## Revisión del 21 de octubre

La [fila del 20, leída el 21](../sources/2026-10-21-farside-flujos-bitcoin.md), contiene doce valores y suma +23,2 millones USD: IBIT +29,9, FBTC +3,6, BITB −10,3, otros nueve 0,0. Es otra sesión respecto al 19; no corrección de la cifra anterior. Revisable, sin conciliación por emisor, sin tendencia o causa de precio demostrada. Una propuesta como PBIT o previsión como JPM no es entrada de capital.

## Revisión del 22 de octubre

La [fila de la sesión del 21](../sources/2026-10-22-farside-flujos-bitcoin.md), consultada el 22, suma +524,8 millones USD; IBIT +235,0 y FBTC +212,7, otros diez +77,1. Doce celdas presentes y aritmética comprobada. Otra sesión, no corrección de la cifra del 20. Dato revisable y sin conciliación por emisor. Aprobación de ETF suizo no equivale a flujos ejecutados.

## Revisión del 23 de octubre

[Sesión del 22](../sources/2026-10-23-farside-flujos-bitcoin.md), consulta del 23: doce cifras presentes, suma −635,6 millones USD. La cobertura parcial de OwlChart (−27,2 a las 22:37 UTC del 22, pocos fondos) no sustituye el agregado completo ni permite fechar la publicación de Farside. Datos revisables sin conciliación por emisor. La sesión del 21 (+524,8) permanece intacta; son días distintos.

## Revisión del 26 de octubre

[Sesión del 23](../sources/2026-10-26-farside-flujos-bitcoin.md), observada del 24 al 26: HODL mantiene guion. Once valores suman −137,9 millones USD, subtotal provisional; un faltante no es cero. Ni total diario ni semana definitivos, aunque medios publiquen agregados. Sin conciliación por emisor o causalidad de precio.
