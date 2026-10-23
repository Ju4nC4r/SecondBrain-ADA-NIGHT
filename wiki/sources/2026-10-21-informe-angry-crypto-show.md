---
title: "Angry Crypto Show — informe del 21 de octubre: procedencia"
type: source
created: "2026-10-21"
updated: "2026-10-21"
tags: [angry-crypto-show, ada, night, transcripcion, procedencia]
sources:
  - "../../raw/notes/2026-10-21-informe-angry-crypto-show.md"
  - "../../raw/notes/2026-10-21-informe-angry-crypto-show-metadatos.json"
  - "../../raw/transcripts/2026-10-20-angry-crypto-show-xAN5CosBIx8.txt"
---

# Angry Crypto Show — informe del 21 de octubre: procedencia

## Originales, fechas y método

[Informe íntegro](../../raw/notes/2026-10-21-informe-angry-crypto-show.md) · [Metadatos, SHA-256 y entrega](../../raw/notes/2026-10-21-informe-angry-crypto-show-metadatos.json) · [Transcripción inglesa automática](../../raw/transcripts/2026-10-20-angry-crypto-show-xAN5CosBIx8.txt) · [Infografía original](../../raw/images/2026-10-21-infografia-angry-crypto-show.png).

- Vídeo: [Strike: «Building A Behemoth.» Charles: «Pogun—1,000x More Efficient Than BitVM.»](https://www.youtube.com/watch?v=xAN5CosBIx8), ID `xAN5CosBIx8`. Publicado el **20 de octubre de 2026, 22:49:01 Europe/Madrid**, 20:49:01 UTC, según metadatos. Duración 10:43; transcripción 00:00–10:42. El orden de las frases del título puede variar.
- Edición del **21 de octubre**, corte de fuentes **08:38 Europe/Madrid**; preparación **08:45:55**. Publicación del episodio, fecha de cada hecho y consulta del informe son hitos distintos.
- La ficha registra envío del 21 a las **08:50:00**, mensaje `1a15d39525dcb5ef`, verificación a las **08:50:47**, con texto e imagen. Archivo y campo de finalización del análisis: **08:52:24**. Se atribuye la comprobación a ese proceso de origen; esta ingesta no accede a Gmail ni reenvía correo.
- Ingesta local: **21 de octubre**. `ingestion_status: pending` y los estados iniciales del original se conservan en RAW como historia; la operación posterior se registra aquí y en el log.

Informe derivado de Codex sobre un canal de opinión. En esta incorporación se leen completos informe, metadatos y TXT y se inspecciona el PNG. La primera exportación de la transcripción falló según el autor y se resolvió abriendo el panel de YouTube; no implica texto ausente en la copia final. No se revisan íntegramente audio/gráficos ni se vuelven a abrir fuentes externas. Las consultas primarias que relata el original se atribuyen a su autor; los artículos completos no están archivados en este conjunto.

Kashi/Kauri se interpreta por contexto como Kalshi y Pogen como Pogun, sin modificar el TXT. **BlockFi en subtítulos frente a Blockenfy en la descripción**, según el informe, sigue sin identificación primaria inequívoca: no se atribuye el supuesto depósito al antiguo prestamista BlockFi.

## Nightmode: anuncio, proveedor y privacidad por tramo

En [03:10–06:47](https://www.youtube.com/watch?v=xAN5CosBIx8&t=190s), el vídeo explica Nightmode y casos de uso futuros. El autor contrasta la [publicación oficial de Midnight del 20](https://midnight.network/blog/nightmode-enables-cross-chain-privacy), **ya incorporada en una ficha propia de la wiki**: [Nightmode, fuente primaria existente](2026-10-21-midnight-nightmode.md). No se crea otro anuncio independiente por repetirlo en el canal.

La arquitectura declarada conserva los activos nativos en bóvedas MPC de su cadena original y representa saldos privados dentro de Midnight. Al operar con Uniswap, el tramo público puede revelar importes; los antecedentes de [SIG Network](../entities/sig-network.md) conservan también tiempos públicos en Ethereum. Desvincular identidad no equivale a invisibilidad total, custodia sin supuestos o seguridad auditada. La frase del vídeo sobre llevar tokens a una bóveda privada «en Midnight» simplifica la distinción entre activo nativo y representación; se conservan ambas formulaciones con sus fuentes.

La [documentación pública de SIG](https://sig.network/index.html) consultada por el autor describe cuentas Ethereum controladas por peticiones de contratos de Midnight y firmantes por umbral. Declara **stagenet disponible**, **mainnet con ledger v9** y **TRON en diciembre de 2026**. Se registra estado/calendario del proveedor, sin operación ejecutada, despliegue general o auditoría propia. La demo en stagenet y la condición de v9 ya figuraban en el [informe del 9](2026-10-09-informe-angry-crypto-show.md); reiterarlas no demuestra otro lanzamiento. El screening anunciado no acredita cumplimiento legal universal.

La [roadmap de Midnight](https://midnight.network/roadmap) consultada por el autor sitúa Collateral Warehouse en **Q1 de 2027**, con varias capacidades de ofertas privadas entre **Q4 de 2026 y Q1 de 2027**. No todas están entregadas. Bitcoin, Solana, préstamos, pagos institucionales, activos reales y liquidez potencial son alcance pretendido, no integraciones o capital captado comprobados. [Offer Files](../concepts/offer-files-y-negociacion-privada.md) y dark pools se describen como intenciones privadas con publicación al casar total/parcialmente; no se acepta la garantía absoluta de que nadie pueda anticiparse o negociar contra el usuario.

## Leios y Pogun: objetivos sin benchmark reproducido

En [01:55–03:09](https://www.youtube.com/watch?v=xAN5CosBIx8&t=115s), el canal atribuye a IOG un inicio de Leios con **3–5x el throughput actual**, después **10–15x condicionado a resultados en mainnet**, y mayores aumentos según demanda, necesidades y economía de operación. Enumera nested transactions, mejoras de cuentas, guard scripts, Plutus V4 y recompensas de staking retirables como cambios previstos del siguiente hard fork. No son activación o prestaciones ya medidas.

El original enlaza [CIP-164](https://cips.cardano.org/cip/CIP-0164) y [sitio técnico de Leios](https://leios.cardano-scaling.org/) para diseño/pruebas; no coteja el hilo original de IOG o los multiplicadores. Se matiza la valoración anterior de escalabilidad infinita sin sustituirla por un resultado experimental. [Leios: estados de evidencia](../concepts/leios-testnet-y-mainnet.md).

[Pogun](../entities/pogun.md) se anuncia para **enero sin año explícito** en el fragmento; enero de 2027 es inferencia contextual, no fecha oficial confirmada. **1.000x frente a BitVM** carece aquí de unidad, versión, carga, hardware y benchmark reproducido: no se transforma en mil veces más TPS de Cardano. En [09:57–10:37](https://www.youtube.com/watch?v=xAN5CosBIx8&t=597s), el presentador recuerda **>600 millones USD en compromisos blandos**; no depósitos, TVL, capital comprometido de forma vinculante o rendimiento conseguido. Su expectativa de instrumentos con rendimiento no identifica producto, tasa, importe o plazo de inversión.

## DeFi: integraciones narradas y métricas pendientes

| Tramo o dato | Afirmación del canal | Límite conservado |
|---|---|---|
| 00:19 y 09:49 | Strike >1.800 millones USD de volumen acumulado y >6.600 operadores únicos | Sin serie, definición de operador o deduplicación reproducidas; no personas, entradas netas o capitalización. |
| 00:27–00:45 | Hackathon el 21 de octubre, 48 horas, 3.000 USD en premios, 10:00 Eastern | Bases y anuncio no verificados. No se convierte la hora sin resolver la zona y horario estacional ni se da por celebrado o pagado. |
| 00:46–00:57 | SundaeSwap permite ADA→sUSDrf | Ruta ejecutable, transacción y condiciones no comprobadas; distinto de integración anterior RealFi/Strike. |
| 00:58–01:10 | RealFi >8,3 millones USD de stablecoins/fondos emitidos, +700.000 en una semana | Serie de Token Terminal no reproducida: emisión, no TVL, ingresos nuevos o capitalización de Strike. |
| 01:11–01:33 | Indigo PSM canjea iUSD/USDrf nominalmente 1:1, sin deslizamiento | Sin transacción o condiciones actuales verificadas; no implica cero comisiones, profundidad ilimitada, solvencia o rescate garantizado. |
| 01:34–01:54 | Asignación empresarial de sUSDrf a Strike | Identidad BlockFi/Blockenfy y movimientos pendientes; no se suman fondos desde una denominación ambigua. |
| 00:05 y 08:27 | ADA en Kalshi >500.000 y luego unos 800.000 USD de volumen | Observaciones distintas del vídeo, sin corte homogéneo reproducido; no se suman o convierten en entradas netas. |

## Contexto externo, discrepancias y continuidad

- **Francia, 07:19–07:42:** el autor consulta la [enmienda I-CF1826](https://www.assemblee-nationale.fr/dyn/17/amendements/3210A/CION_FIN/CF1826): adopción en comisión el **7 de octubre**, propuesta sobre ciertos tokens de dinero electrónico con aplicación propuesta desde 2027. **31,4 % no figura en el texto consultado** ni acredita ley vigente o ámbito idéntico para todos los stablecoins. Es el mismo expediente ya recogido en el [informe del 15](2026-10-15-informe-angry-crypto-show.md), no novedad legislativa del 20. No se actualiza aquí el derecho vigente ni se da una conclusión fiscal al lector.
- **Saylor y J.P. Morgan, 06:56–07:11:** volver a seis cifras y superar acciones/oro/inmuebles a diez años son previsiones atribuidas, sin entrevista o informe original cotejados en este análisis. La [ficha primaria de JPM ya existente](2026-10-21-jpmorgan-previsiones-bitcoin.md) documenta un rango de previsiones y ausencia de asignación de cartera; no confirma por extensión la comparación precisa del vídeo o rentabilidades garantizadas. No se duplica ese comunicado como anuncio nuevo.
- **Citi/Aave y supuesto primer ETF spot minorista en Suiza, 06:49–07:18:** sin documentos primarios suficientes. ETF y ETP no se equiparan ni se valida «primero» por el titular. No se sustituye esa laguna por la propuesta PBIT de otro informe.

## Opiniones y publicidad

| Tramo | Atribución | Condiciones y campos ausentes |
|---|---|---|
| 08:48–09:18 | Presentador optimista para altcoins/ADA en Q4 pese a mercado irregular | Escenario condicional para el resto del trimestre, sin entrada, objetivo, stop, asignación o probabilidad. ADA cerca de 0,22 USD es lectura de la grabación, no cotización actual verificada. No se heredan niveles de episodios anteriores. |
| 09:19–09:56 | Aprobación editorial de Strike/RealFi | Sin orden concreta de compra o depósito ni rentabilidad objetivo; métricas no auditadas. |
| 09:57–10:37 | Potencial institucional/minorista de Pogun | Sujeto a lanzamiento y eficiencia no contrastados; sin producto, tasa, importe o plazo recomendado. |
| 07:43–08:47 | Kalshi, segmento patrocinado dirigido a estadounidenses | Alega regulación CFTC, unos 19 mercados y apalancamiento «razonable». Términos y elegibilidad actuales no verificados; no recomendación propia o validación para España. Apalancamiento amplifica pérdidas. |

## Integridad y registro

Informe, PNG y TXT coinciden en tamaños y SHA-256 con los metadatos. PNG **1024 × 1536** inspeccionado: «Documentado» remite al contraste del autor, no a verificación nueva del funcionamiento. La imagen distingue anuncio y despliegue, privacidad por tramo, stagenet/v9, Pogun sin benchmark, compromisos blandos, emisión frente a TVL, opiniones y patrocinio. Los originales permanecen intactos.

[Síntesis de la wiki](../reports/2026-10-21-angry-crypto-show.md) · [Informe anterior](2026-10-20-informe-angry-crypto-show.md) · [Seguimiento del canal](../topics/seguimiento-angry-crypto-show.md).
