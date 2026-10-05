---
title: "Fuentes para contrastar mercado, adopción y uso de Cardano y Midnight"
type: report
created: "2026-10-05"
updated: "2026-10-05"
tags: [cardano, midnight, datos, metodologia]
capture_timezone: "Europe/Madrid"
cutoff: "2026-10-05T09:35:56+02:00"
author: "Codex, informe elaborado a petición del usuario"
status: "catálogo de fuentes y metodología verificados"
---

# Fuentes para contrastar mercado, adopción y uso de Cardano y Midnight

## Pregunta y resultado

¿Qué fuentes primarias y series históricas permiten contrastar mercado, adopción y utilización de la red?

Se identifican fuentes para obtener datos de cadena, negociación, derivados y fondos. **Precio, volumen de negociación, uso del protocolo y adopción deben medirse por separado.** Este informe verifica documentación y disponibilidad descrita de las fuentes; no descarga todavía una serie histórica completa ni confirma las cotizaciones del informe previo de las 07:39.

Creación y captura: 5 de octubre de 2026. Corte: 09:35:56, Europe/Madrid. Las fechas internas y de acceso de las fuentes se distinguen en el catálogo. La fecha de publicación de las páginas de API que no muestran una fecha verificable queda sin determinar.

## Catálogo contrastado

| Ámbito | Fuente y tipo | Serie o evidencia que permite construir | Límites |
|---|---|---|---|
| Cardano, actividad y participación | [Cardano Docs: mantenimiento](https://docs.cardano.org/stake-pool-operators/maintenance), documentación oficial | La página remite a cardano-node, cardano-db-sync y cardano-graphql para datos de blockchain. Con una fuente sincronizada pueden elaborarse recuentos de bloques y transacciones, actividad de direcciones y participación por época. | Deben documentarse consultas, versión y punto de sincronización. Direcciones o transacciones no equivalen a personas. Las métricas propuestas son elaboración de este informe, no cifras publicadas en la página. |
| Midnight, historia pública | [Notas del Indexer](https://docs.midnight.network/relnotes/midnight-indexer) y [API v4, release 4.1.0](https://docs.midnight.network/relnotes/midnight-indexer/midnight-indexer-4-1-0), documentación oficial | Historia de bloques, transacciones y acciones de contratos; la release 4.1.0 documenta el campo fee calculado con el ledger y consultas para sincronizar estado protegido y DUST. | Seleccionar esquema y versión compatibles con el nodo. El indexador representa una vista derivada de la cadena; hay que guardar hashes y verificar finalización. No se declara que 4.1.0 sea la release actual para mainnet. |
| Midnight, acceso al proveedor | [Entornos y endpoints](https://docs.midnight.network/relnotes/network), documentación oficial actualizada el 2 de octubre | La referencia identifica Mainnet, Preview y Preprod y señala la migración de Mainnet a Blockfrost tras el 30 de septiembre. | Mainnet requiere token de proyecto. No se realizó consulta autenticada ni se probó cobertura histórica. No mezclar actividad de redes de prueba con uso real de Mainnet. |
| Precios y negociación en un mercado | [Coinbase Exchange: velas históricas](https://docs.cdp.coinbase.com/api-reference/exchange-api/rest-api/products/get-product-candles), documentación primaria de un mercado | Velas con tiempo, apertura, máximo, mínimo, cierre y volumen por producto. Permite contrastar la negociación del par que se compruebe disponible. | Hasta 300 velas por consulta; intervalos sin operaciones pueden faltar. Verificar listado del par y fechas antes de usarlo para ADA o NIGHT. No representa todos los mercados ni reproduce automáticamente un precio agregado. |
| Mercado agregado | [CoinGecko: rango histórico por ID](https://docs.coingecko.com/reference/coins-id-market-chart-range), documentación del agregador | Arrays fechados de precios, capitalización y volumen total. Identificar activos por ID y, cuando corresponda, contrato o política. | Es una serie calculada por un proveedor, no datos primarios de cada operación. Plan, granularidad y cobertura condicionan el acceso; el volumen publicado no debe sumarse mecánicamente como si cada punto fuera volumen exclusivo del intervalo. |
| Derivados de ADA | [CoinGlass: OI OHLC](https://docs.coinglass.com/reference/oi-ohlc-histroy), documentación del agregador | Interés abierto histórico por par, mercado e intervalo; el [catálogo](https://docs.coinglass.com/reference/endpoint-overview) distingue historia agregada, margen en moneda y stablecoin. | Registrar exchanges incluidos, unidad, denominación y valoración. No se obtuvo una respuesta API que confirme los 615 millones y +15 % del informe inicial. No sustituye el dato primario de cada exchange. |
| Flujos de ETF de Bitcoin | [Farside: tabla histórica](https://farside.co.uk/bitcoin-etf-flow-all-data/), agregador, y [BlackRock: IBIT](https://www.ishares.com/us/products/333011/ishares-bitcoin-trust-etf), emisor | Farside separa fondos y sesiones; BlackRock permite descargar NAV y participaciones históricas de IBIT. Se obtuvo su exportación oficial, archivada en RAW/data. | Farside e iShares no son dos fuentes independientes para todos los fondos. El flujo diario y el cambio de participaciones requieren conciliación de fechas y metodología; véase el [informe IBIT](2026-10-05-ibit-conciliacion-flujos-etf.md). |
| Adopción y privacidad | [Flujo de contratos Midnight](https://docs.midnight.network/guides/deploy-and-operate), documentación oficial | Distingue datos públicos consultados al indexador de estado privado local. Proporciona una base para definir métricas públicas de llamadas y despliegues. | El estado privado no permite contar usuarios reales desde la cadena sin evidencia adicional. Ejemplos, anuncios o repositorios no demuestran despliegues activos ni usuarios pagadores. |

## Diseño de un conjunto de datos reproducible

Propuesta de elaboración, aún sin ejecutar una descarga masiva:

1. Para cada observación guardar activo e identificador, red, métrica, valor, unidad, intervalo observado y fuente. Mantener UTC para cálculo y Europe/Madrid para presentación.
2. Conservar respuesta original, URL o consulta, parámetros, versión, instante de captura y huella. En datos de cadena añadir bloque o época, hash y criterio de finalización.
3. Etiquetar valores observados, derivados, provisionales, revisados y ausentes. Un campo vacío no se convierte en cero.
4. Separar transacciones de usuario, operaciones del sistema, despliegues y llamadas; definir qué se incluye antes de comparar Cardano y Midnight.
5. Para demanda y adopción, combinar actividad recurrente de contratos con evidencia verificable de aplicaciones operativas. No utilizar precio, número de wallets o descargas como sustituto automático de usuarios.
6. En derivados, distinguir OI de volumen y separar cambios en contratos de cambios en su valoración en USD. En ETF, usar sesiones bursátiles y metodología de creación/redención.
7. Relacionar anuncios con fecha de publicación, fecha efectiva y primera captura para evitar presentar como nuevo un hecho repetido.

Un análisis de relación entre mercado y uso requiere ventanas alineadas y control de cambios de cobertura. La correlación temporal por sí sola no establece causalidad.

## Lagunas que siguen abiertas

No se ha reconstruido la fotografía exacta de CoinMarketCap del informe inicial, porque carece de un corte final y de respuestas fechadas archivadas. Tampoco se han descargado series completas de uso, adopción u OI. Se ha resuelto qué fuentes y qué condiciones permiten hacerlo; las afirmaciones de mercado anteriores permanecen atribuidas hasta contrastarlas con datos compatibles.

Los metadatos de documentación consultada están en la [nota de fuentes](../notes/2026-10-05-fuentes-investigacion-overview.md). La documentación de acceso no confirma por sí sola el estado ni la utilización actual de una red.

