# Registro de fuentes de las tres preguntas abiertas

Captura: 2026-10-05, corte 09:35:56, Europe/Madrid. Nota de consulta elaborada por Codex; no es una copia íntegra de las páginas web. Los códigos originales y la exportación del emisor sí se conservan en RAW.

## Documentación de Midnight

Páginas consultadas: [notas del nodo](https://docs.midnight.network/relnotes/node), [Kachina](https://docs.midnight.network/concepts/kachina), [DUST](https://docs.midnight.network/concepts/dust-architecture), [BST](https://docs.midnight.network/concepts/blockchain-space-tokenization), [sidechains](https://docs.midnight.network/concepts/sidechains-partnerchains), [entornos](https://docs.midnight.network/relnotes/network) y [flujo de contratos](https://docs.midnight.network/guides/deploy-and-operate). Las páginas conceptuales y la referencia de entornos muestran actualización del 2 de octubre de 2026; esa fecha no es necesariamente su primera publicación. El artículo histórico de [IOG](https://www.iog.io/news/from-research-to-reality-building-midnight-on-peer-reviewed-foundations) está fechado el 6 de marzo de 2026.

Las [notas del indexador](https://docs.midnight.network/relnotes/midnight-indexer) y la [release 4.1.0](https://docs.midnight.network/relnotes/midnight-indexer/midnight-indexer-4-1-0), fechada el 20 de abril de 2026, se consultaron para conocer los campos disponibles, sin certificar compatibilidad de cada release con la red en producción. Se guardó el [código fijado y sus metadatos](../repos/2026-10-05-midnight-implementacion/procedencia.md).

## Datos y metodologías

- [Cardano: mantenimiento](https://docs.cardano.org/stake-pool-operators/maintenance): documentación oficial de componentes para acceder a la cadena; fecha de publicación no determinada.
- [Coinbase: velas](https://docs.cdp.coinbase.com/api-reference/exchange-api/rest-api/products/get-product-candles): documentación primaria del mercado; fecha de publicación no determinada. No se descargaron velas.
- [CoinGecko: rango histórico](https://docs.coingecko.com/reference/coins-id-market-chart-range): documentación del agregador; fecha de publicación no determinada. No se descargó una serie de precios.
- [CoinGlass: OI OHLC](https://docs.coinglass.com/reference/oi-ohlc-histroy) y [catálogo](https://docs.coinglass.com/reference/endpoint-overview): documentación del agregador; fecha de publicación no determinada. No se realizó consulta autenticada de OI.
- [Farside reciente](https://farside.co.uk/btc/) y [histórico](https://farside.co.uk/bitcoin-etf-flow-all-data/): ambas conservan ausente IBIT del 2 de octubre al corte. Las filas se transcribieron a [CSV](../data/2026-10-05-farside-etf-1-2-octubre.csv). La fecha del hecho es la sesión bursátil; la hora de publicación no está indicada.
- [BlackRock: IBIT](https://www.ishares.com/us/products/333011/ishares-bitcoin-trust-etf): fuente primaria del emisor, datos de la ficha al 2 de octubre y [exportación original](../data/2026-10-05-ibit-exportacion-blackrock.xls), con filas históricas fechadas. Los [metadatos](../data/2026-10-05-etf-procedencia.json) conservan la URL de descarga y la huella.

## Informes producidos

- [Contraste científico y técnico](../reports/2026-10-05-midnight-fundamentos-implementacion.md).
- [Fuentes de mercado, adopción y uso](../reports/2026-10-05-fuentes-mercado-adopcion-uso.md).
- [Conciliación de IBIT](../reports/2026-10-05-ibit-conciliacion-flujos-etf.md).

