---
title: "Fuentes para medir mercado, adopción y uso"
type: report
created: "2026-10-05"
updated: "2026-10-05"
tags: [cardano, midnight, fuentes, metricas]
sources:
  - "../sources/2026-10-05-fuentes-mercado-adopcion-uso.md"
---

# Fuentes para medir mercado, adopción y uso

**Corte: 5 de octubre de 2026, 09:35:56, Europe/Madrid.** [Informe completo y catálogo](../../raw/reports/2026-10-05-fuentes-mercado-adopcion-uso.md) · [Procedencia](../sources/2026-10-05-fuentes-mercado-adopcion-uso.md).

## Resultado

Se identificaron fuentes verificables para construir series, con funciones distintas:

- **Cadena Cardano:** cardano-node, db-sync y GraphQL, referidos por la documentación oficial. Las series deben indicar consultas, época/bloque, versión, sincronización y finalización.
- **Cadena Midnight:** nodo e indexador para bloques, transacciones y acciones públicas. El esquema debe corresponder a las versiones utilizadas. Mainnet tiene acceso público documentado mediante Blockfrost con token; no se realizó consulta autenticada.
- **Negociación primaria:** API de un exchange, como velas de Coinbase para un par cuyo listado se verifique. Un solo mercado no representa un precio agregado.
- **Mercado agregado:** CoinGecko ofrece series de precio, capitalización y volumen con identificadores y granularidad específicos; es un agregador.
- **Derivados:** CoinGlass distingue OI de volumen y ofrece historia por par o agregada; hace falta documentar exchanges, unidades y cobertura. Los 615 millones de ADA del informe inicial siguen sin contrastar.
- **ETF:** tablas por sesión de Farside y NAV/participaciones del emisor, con conciliación de fechas. Se archivaron filas de Farside y la exportación de IBIT.

Cada afirmación remite al [catálogo con enlaces externos y límites](../../raw/reports/2026-10-05-fuentes-mercado-adopcion-uso.md) y al [registro de consulta](../../raw/notes/2026-10-05-fuentes-investigacion-overview.md). La fecha de publicación de páginas que no la muestran permanece sin determinar.

## Interpretación

No basta un repunte de precio, volumen o interés abierto para afirmar mayor uso o adopción. Las transacciones y direcciones tampoco equivalen a usuarios: operaciones del sistema, automatización y actividad repetida requieren clasificación. En Midnight, el estado privado local limita lo observable públicamente.

La metodología propuesta conserva intervalos y tiempos de captura, respuestas originales, unidades, identificadores, revisiones y ausencias. Evita mezclar Mainnet con redes de prueba o sumar puntos de volumen de ventanas solapadas. Véase [métricas de uso y adopción](../concepts/metricas-de-uso-y-adopcion.md).

## Estado de la pregunta

**Fuentes y método identificados; series empíricas pendientes.** No se descargó una historia completa de actividad, adopción, precios u OI. Las cotizaciones del primer informe conservan su estado histórico y atribuido; no se reemplazan con lecturas posteriores.

[Seguimiento de mercado](../topics/seguimiento-mercado-ada-night.md) · [Cardano / ADA](../entities/cardano-ada.md) · [Midnight / NIGHT](../entities/midnight-night.md) · [Índice de informes](index.md).

