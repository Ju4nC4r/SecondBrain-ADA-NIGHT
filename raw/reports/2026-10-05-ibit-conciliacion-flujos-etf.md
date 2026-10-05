---
title: "IBIT: conciliación del flujo pendiente y total provisional de ETF"
type: report
created: "2026-10-05"
updated: "2026-10-05"
tags: [bitcoin, ibit, etf, datos-provisionales]
capture_timezone: "Europe/Madrid"
cutoff: "2026-10-05T09:35:56+02:00"
author: "Codex, informe elaborado a petición del usuario"
status: "dato definitivo pendiente; fuentes contrastadas"
---

# IBIT: conciliación del flujo pendiente y total provisional de ETF

## Pregunta y resultado

¿Cómo completar el dato pendiente de IBIT conservando la distinción entre la cifra provisional y la definitiva?

**Al corte Farside aún muestra IBIT del 2 de octubre como ausente.** Se comprobaron su tabla reciente y la histórica. Se conserva el agregado de 134,4 millones de USD como provisional. Se descargó además la exportación oficial de BlackRock: permite calcular una aproximación por cambio de participaciones, pero no confirma el dato diario faltante de Farside ni permite sustituirlo como cifra definitiva.

Creación y captura: 5 de octubre de 2026, corte 09:35:56 de Madrid. Fechas de las sesiones examinadas: 1 y 2 de octubre de 2026. Las páginas de datos son dinámicas; no se conoce su hora exacta de publicación.

## Qué es IBIT y qué dato falta

IBIT es el símbolo de [iShares Bitcoin Trust ETF, de BlackRock](https://www.ishares.com/us/products/333011/ishares-bitcoin-trust-etf), negociado en NASDAQ. Su objetivo declarado es seguir el precio de bitcoin. El dato pendiente del informe es el **flujo neto diario**, no el precio de la participación, el volumen negociado o el patrimonio del fondo.

## Fotografía de Farside

Fuentes: [tabla reciente](https://farside.co.uk/btc/) y [tabla de todas las sesiones](https://farside.co.uk/bitcoin-etf-flow-all-data/), consultadas el 5 de octubre. La [transcripción de las dos filas](../data/2026-10-05-farside-etf-1-2-octubre.csv) conserva todas las columnas, el signo y el dato ausente, con sus [metadatos](../data/2026-10-05-etf-procedencia.json).

| Sesión | IBIT, millones USD | Total mostrado, millones USD | Estado |
|---|---:|---:|---|
| 2026-10-01 | 195,6 | 102,7 | Valores publicados por Farside; no auditados contra cada emisor |
| 2026-10-02 | Ausente, guion en la fuente | 31,7 | Parcial: IBIT todavía no publicado |

La suma 102,7 + 31,7 = **134,4** coincide con el [informe inicial conservado](2026-10-05-informe-ada-night-bitcoin.md). Los demás valores de la segunda fila suman 31,7. Ese acuerdo aritmético no transforma la ausencia de IBIT en cero ni hace definitivo el total. No se afirma que no hubiera flujo.

## Datos primarios de BlackRock y aproximación

Se conserva sin modificar la [exportación oficial](../data/2026-10-05-ibit-exportacion-blackrock.xls), enlazada desde la ficha del emisor. Aunque su extensión es XLS, el contenido es XML Spreadsheet; se extrajeron las filas de la hoja Historical sin alterar el original. La [selección trazable](../data/2026-10-05-ibit-datos-seleccionados.json) distingue estos datos de un flujo publicado.

| Fecha de la hoja Historical | NAV por participación, USD | Participaciones en circulación |
|---|---:|---:|
| 2026-09-30 | 47,393896 | 1.414.960.000 |
| 2026-10-01 | 47,934783 | 1.414.760.000 |
| 2026-10-02 | 47,637156 | 1.418.840.000 |

**Cálculo propio, aproximado:** variación de participaciones entre el 1 y el 2 de octubre × NAV del 2 = 4.080.000 × 47,637156 = 194.359.596,48 USD, aproximadamente **194,4 millones**. Es una aproximación al valor de emisión neta reflejado por esos saldos; no una publicación del flujo IBIT correspondiente a la sesión faltante.

Hay una discrepancia temporal o metodológica que impide cerrar la conciliación: aplicado a la variación del 30 de septiembre al 1 de octubre, el mismo cálculo da −9.586.956,60 USD, mientras Farside publica +195,6 millones para IBIT el 1 de octubre. No se ha identificado la causa. Podrían intervenir fecha de negociación/liquidación o convenciones de corte, pero son hipótesis, no hechos comprobados.

Por ello **no se añade automáticamente 194,4 al total de 134,4**. Tampoco se interpreta el cambio de patrimonio o de volumen como flujo: ambas magnitudes incorporan otros efectos.

## Procedimiento de cierre y conservación del historial

1. Cuando se publique IBIT del 2 de octubre en una fuente con metodología y sesión identificadas, guardar una nueva captura y su relación con esta. No sobrescribir el informe inicial ni esta fotografía.
2. Verificar fecha de sesión, unidad y si hubo revisiones de otras columnas o de la fila del 1 de octubre.
3. Recalcular cada total con todas las columnas actualizadas, permitiendo diferencias de redondeo. Si solo cambia IBIT del 2, el nuevo agregado será 134,4 millones más ese valor; si cambian otras celdas, recalcular desde las filas revisadas.
4. Etiquetar por separado publicado por proveedor, calculado por la wiki y conciliado contra emisor. La palabra definitivo exige un criterio de cierre; una cifra publicada también puede revisarse.
5. Actualizar la wiki con los valores anterior y nuevo, fecha de captura y explicación. La fuente anterior conserva su estado provisional histórico.

Se ha comprobado el estado pendiente y aportado una fuente primaria para investigarlo. Falta una conciliación de metodología y fechas o la publicación del proveedor; no se inventa un valor para cerrar la pregunta.

