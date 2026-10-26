# Angry Crypto Show — Informe diario — 24 de octubre de 2026

**Entrega retrasada.** La revisión iniciada el 24 quedó incompleta por tiempos de espera en la comprobación automática del navegador y una posterior desconexión. La transcripción y el contraste se completan el **26 de octubre, 07:52, Europe/Madrid (CET, UTC+1)**. La fecha de informe se conserva como 24; no se afirma que se entregara ese día. Este documento cubre el vídeo identificado en la revisión del 24 y no sustituye una revisión del canal correspondiente al 25 o 26.

## Vídeo y método

[Charles: «Cardano—Infinitely Scalable. Unbelievable Innovations Coming.» Angry Crypto Reacts](https://www.youtube.com/watch?v=IltXg8rmF-8). Publicado el **23 de octubre de 2026 a las 23:38:51 de Madrid** (21:38:51 UTC). Duración: **10:37 en el reproductor; 10:38 en metadatos**.

Se leyó la **transcripción original completa de YouTube, automática en inglés, de 00:00 a 10:35**, exportada desde la sesión autorizada de Brave y resumida en español. No se revisaron íntegramente audio ni gráficas. Hay posibles errores de reconocimiento en nombres y cifras, especialmente el nombre de una plataforma de perpetuos y la cotización abreviada de BTC. No se reconstruyen datos ambiguos por intuición.

## Resumen

- **Escalabilidad:** Hoskinson describe una visión combinada Leios/Hydra. Las cifras extremas son declaraciones o simulaciones atribuidas; no rendimiento de mainnet demostrado aquí. La especificación de Linear Leios obliga a comparar tamaño y complejidad de transacciones, no solo TPS.
- **MiCA:** existe una respuesta oficial de Cardano Foundation, presentada el **30 de septiembre** y publicada el **21 de octubre**. Defiende regulación proporcional y distinguir staking directo de servicios con custodia. Es una posición en consulta, no un cambio legal aprobado.
- **Gobernanza:** el presentador anuncia que probablemente votará **NO** a la propuesta de reserva de cobre por **22 millones ADA**. No confirma un voto ya emitido ni una decisión de la comunidad.
- **RealFi y desarrolladores:** las métricas de emisión y holders quedan atribuidas; la existencia de Blaster está documentada, pero las correcciones recientes y primera versión de Hades citadas por el canal no se comprobaron mediante una versión o commit específico.

## Noticias y contraste

**00:05–00:24 — RealFi y ADA envuelta.** El canal atribuye a Token Terminal más de **8,4 millones USD** emitidos en stablecoins y fondos tokenizados, +100.000 USD en 72 horas, y más de **6.900 holders** de ADA envuelta por Coinbase. No se reprodujeron las series ni el contrato/red del contador. Emisión no equivale a TVL; direcciones o holders no equivalen necesariamente a personas o demanda nueva acreditada.

**00:26–00:58 — Blaster/Hades.** El [artículo técnico oficial de IO sobre verificación automática](https://www.iog.io/news/automated-formal-verification-for-cardano-smart-contracts) describe herramientas Lean 4 para verificar propiedades de contratos y generar contraejemplos. El [programa High Assurance](https://www.iog.io/news/cardano-high-assurance-formal-verification) contempla un entorno de desarrollo en contenedor y entregas por fases. Esas publicaciones respaldan el proyecto, pero no acreditan por sí solas el parche o primera versión de Hades mencionado como novedad. Una prueba formal demuestra propiedades dentro de su especificación y supuestos; no certifica ausencia universal de errores o riesgos económicos.

**01:00–01:17 — Perpetuos ADA.** La transcripción identifica KuCoin y un volumen superior a **1,1 millones USD**, frente a otras monedas. No se verificaron plataforma mostrada, ventana exacta, puesto en el ranking ni valores comparables. No se mezcla este dato con Polymarket/Kalshi de los informes anteriores ni se interpreta volumen como entradas netas de capital.

**01:18–03:28 — Leios, Hydra y afirmaciones tecnológicas.** El vídeo atribuye a Hoskinson decenas o cientos de miles de TPS con Leios, más de un millón en simulación de Hydra, un nuevo lenguaje y la resolución del trilema. La [CIP-0164 oficial](https://cips.cardano.org/cip/CIP-0164), todavía propuesta, subraya que TPS aislado es inadecuado: en sus escenarios, **140.000–300.000 bytes de transacciones por segundo** se relacionan aproximadamente con **100–200 TPS de transacciones medias**, no con cientos de miles de TPS. Son unidades y condiciones distintas. Sus simulaciones y estimaciones no garantizan resultados de producción.

El [sitio técnico de Leios](https://leios.cardano-scaling.org/) presenta el entorno de pruebas. Hydra es un modelo de canales fuera de cadena por aplicación; su rendimiento no se suma automáticamente al de la cadena base. No se reprodujo el benchmark del millón ni se cotejó la entrevista original completa. **Escalabilidad infinita, resolución del trilema e innovaciones futuras permanecen afirmaciones atribuidas**, sin convertirlas en capacidad ilimitada actual o garantía de seguridad.

**03:31–05:08 — Nightmode, activos e interoperabilidad.** El presentador reitera el plan TRON para diciembre y una posibilidad de atraer **10 billones USD** de activos mediante divulgación selectiva; también expresa buena valoración de Filecoin y cita 2,2 billones USD de transferencias trimestrales de stablecoins en TRON. Estas dos cifras no se verificaron y no son activos ya captados por Midnight. La [página de SIG](https://sig.network/index.html), consultada el 26, sigue separando stagenet, mainnet con ledger v9 y TRON previsto en diciembre de 2026. No se afirma retrospectivamente una entrega operativa el 24. Screening y privacidad no garantizan cumplimiento legal universal. La relación exacta con Filecoin no se comprobó mediante un anuncio o contrato primario.

**05:10–06:42 — Consulta MiCA.** La [publicación oficial de la Fundación](https://cardanofoundation.org/blog/mica-review-consultation-response) confirma que presentó su respuesta el **30 de septiembre** y la explicó el **21 de octubre**. Propone mantener neutralidad tecnológica, proporcionalidad y enfoque por funciones y riesgos; distingue delegación directa sin custodia del staking intermediado. Pide claridad y evitar regímenes innecesarios para actividades descentralizadas. **Es una aportación al debate regulatorio**, no una exención nueva, una decisión de la Comisión ni asesoramiento jurídico para el lector.

**06:44–07:07 — Otros titulares.** Recoge una frase de CZ sobre comprar cuando se declara muerto a Bitcoin y oposición de varias empresas a la tokenización de sus acciones en OKX. No se cotejaron las declaraciones ni las comunicaciones corporativas originales. La frase de CZ es una opinión atribuida sin entrada, plazo o control de riesgo; no una pauta propia de inversión.

## Recomendaciones, opiniones y promoción

| Tema y momento | Acción o lectura del autor | Condiciones, horizonte y límites |
|---|---|---|
| Reserva estratégica de cobre, 08:46–10:26 | Como DRep, anticipa aproximadamente un 99% de inclinación a votar NO a la solicitud de 22 millones ADA | Intención provisional: aún prepara su justificación y pide opiniones. Cree que encaja peor que stablecoins, swaps y DeFi. No se verificó su voto on-chain, el cómputo actual ni el plazo exacto. |
| ADA/XRP y privacidad, 07:41–08:44 | Mantiene optimismo por desarrollos y narrativas; seguirá observando el mercado | Sin compra/venta concreta, objetivo, stop, asignación ni fecha de recuperación. ADA por encima de 0,21 USD pertenece a la grabación, no es cotización actual verificada. |
| Kalshi, 07:08–07:38 | Promoción patrocinada de perpetuos, bono y enlace para usuarios de EE. UU. | Elegibilidad y condiciones actuales no comprobadas; no se valida acceso desde España. El apalancamiento amplifica pérdidas. |

El [anuncio del debate de gobernanza en el foro Cardano](https://forum.cardano.org/t/governance-hour-12-cardano-strategic-copper-reserve-22m-rwa-tokenization-27-october/157519) identifica a **Toto Finance** y la solicitud de **22 millones ADA**. Respalda que la propuesta se discute, no que haya sido aprobada, desembolsada o rechazada. El sentimiento comunitario descrito por el autor no es una encuesta representativa comprobada. La referencia relativa a unas tres semanas o 24 días corresponde a la grabación y no se usa como fecha límite actual.

## Registro de entrega

La fecha de publicación, la del informe y las de preparación/envío se registran separadamente. Se conservan transcripción automática original e infografía. Gmail y archivo RAW se verifican por separado; la ingesta de la wiki solo se confirmará con evidencia. No se hace commit ni push. La revisión completa del 23 ya archivada no se reenvía sin la respuesta del usuario a la pregunta de entrega adicional.
