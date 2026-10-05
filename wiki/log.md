# Registro de actividad

## [2026-10-02] init | Estructura inicial de SecondBrain-CryptoADA

- Creadas las capas de fuentes originales, wiki y esquema de mantenimiento.
- Añadidos índices, visión general y plantillas.
- Conservados el documento original de Karpathy y su traducción en la raíz.
- Creada la página de referencia de la guía; no se han incorporado noticias ni cotizaciones.
- Inicializado el control de versiones local, sin remoto ni publicación.

## [2026-10-05] archive | Copia del informe de ADA, NIGHT y Bitcoin en RAW

- Fuente: informe ampliado del 5 de octubre procedente del chat «Informe diario de noticias de ADA y NIGHT»; consultas declaradas desde las 07:39 de Madrid, sin hora final de corte.
- Operación: copia puntual solicitada por el usuario en `raw/reports/`; cuerpo conservado sin cambios, extrayendo únicamente la directiva de presentación de la interfaz.
- Añadidos [informe original](../raw/reports/2026-10-05-informe-ada-night-bitcoin.md), [metadatos](../raw/reports/2026-10-05-informe-ada-night-bitcoin-metadatos.md) y [resumen de procedencia](sources/2026-10-05-informe-ada-night-bitcoin.md).
- Actualizados el índice general, el índice de fuentes y la visión general.
- No se han vuelto a verificar las cifras ni se han capturado los artículos externos completos. Bitcoin se conserva como parte del documento copiado, sin ampliar por sí solo el alcance de la wiki.
- No se ha modificado la automatización diaria ni su chat de destino.
- Revisión de coherencia: comprobados los enlaces Markdown locales de las 14 páginas de la wiki y de los informes en RAW; no se encontraron enlaces rotos. La comparación confirmó que el cuerpo de la copia coincide con el del informe extraído. La validez de las afirmaciones externas queda pendiente de una nueva consulta de sus fuentes.

## [2026-10-05] ingest | Integración del informe archivado en la wiki

- Fuente: [informe de ADA, NIGHT y Bitcoin conservado en RAW](../raw/reports/2026-10-05-informe-ada-night-bitcoin.md), con su [nota de procedencia](../raw/reports/2026-10-05-informe-ada-night-bitcoin-metadatos.md).
- Creada [síntesis diaria](reports/2026-10-05-seguimiento-ada-night-bitcoin.md) y páginas de [Cardano / ADA](entities/cardano-ada.md), [Midnight / NIGHT](entities/midnight-night.md) y [Bitcoin / BTC](entities/bitcoin-btc.md).
- Añadidos los conceptos [interés abierto en futuros](concepts/interes-abierto-en-futuros.md) y [flujos de ETF de Bitcoin](concepts/flujos-etf-bitcoin.md), limitados a su uso documentado, y el tema [seguimiento de mercado](topics/seguimiento-mercado-ada-night.md).
- Actualizados el resumen de fuente, el índice general, los índices de categoría y la visión general.
- Conservadas las cotizaciones como fotografías históricas atribuidas al informe y el total de ETF como provisional. No se han vuelto a consultar las fuentes externas en esta incorporación.
- No había afirmaciones de mercado anteriores integradas que sustituir; quedan pendientes fuentes independientes para confirmar, corregir o documentar contradicciones.
- Revisión de coherencia: comprobadas 21 páginas Markdown de la wiki y de informes en RAW; sin enlaces locales rotos ni páginas de la wiki sin enlaces entrantes. Las huellas de los dos archivos originales de RAW no han cambiado. Las páginas documentan los datos históricos, cifras provisionales y lagunas metodológicas; falta verificación externa independiente.

## [2026-10-05] automation | Archivo diario e integración en la LLM Wiki

- Actualizada la automatización existente «Noticias diarias de ADA, NIGHT y Bitcoin» para añadir el guardado en este proyecto y la integración de futuras entregas en fuentes, informes, entidades, conceptos y temas de la wiki.
- Conservados el horario diario de las 07:00 de Madrid, el estado activo y el chat de entrega «Informe diario de noticias de ADA y NIGHT».
- Añadidas instrucciones de no sobrescribir originales, evitar duplicados, conservar procedencia y fechas, señalar contradicciones y comprobar enlaces.
- Verificada la configuración persistida. No se ha ejecutado de nuevo el informe de hoy; la primera ejecución automática con el flujo completo queda pendiente de comprobación.

## [2026-10-05] ingest | Bibliografía científica y técnica de Midnight y NIGHT

- Lote solicitado por el usuario: siete PDF completos en `raw/articles`, manteniendo originales sin modificar y metadatos de captura, versión y SHA-256.
- Selección: cinco trabajos vinculados por IOG a los fundamentos de Midnight, más Nightpaper y whitepaper de tokenomics 1.81. Dos copias académicas son preprints de trabajos publicados posteriormente.
- Añadidos [bibliografía](../raw/articles/2026-10-05-midnight-bibliografia.md), manifiesto, siete fichas en `wiki/sources`, [tema](topics/midnight-fundamentos-cientificos.md), [entidad](entities/midnight-night-dust.md) y [concepto](concepts/modelo-token-recurso.md).
- Actualizados los índices general y de categorías y la visión general; conservadas las entradas históricas y el informe previo.
- Documentada la diferencia entre deflación en Nightpaper y expansión desinflacionaria de oferta circulante en whitepaper. No se equiparan resultados teóricos con auditoría del protocolo ni con valoración de NIGHT.
- Revisión de coherencia: PDF abiertos y páginas de título inspeccionadas, hashes registrados y enlaces locales comprobados; sin enlaces rotos ni nuevas páginas huérfanas en el lote.

## [2026-10-05] verify | Cinco artículos científicos descargados en RAW

- La comprobación de la carpeta confirmó que los cinco trabajos científicos de la [bibliografía de Midnight](../raw/articles/2026-10-05-midnight-bibliografia.md) ya tenían sus PDF completos y notas de procedencia en `raw/articles/`, además de los dos documentos oficiales del proyecto.
- Verificados el encabezado PDF, el tamaño y la coincidencia SHA-256 de los cinco trabajos con el manifiesto de captura; todas las comprobaciones fueron satisfactorias.
- Comprobados los enlaces Markdown locales de RAW y de la wiki; no se encontraron enlaces rotos.
- No se han duplicado descargas ni modificado o movido los originales existentes. Las fichas de fuente y la síntesis científica ya estaban integradas en la wiki.

## [2026-10-05] link | Asociación de los cinco trabajos con el seguimiento de Midnight

- Comprobadas las cinco fichas de fuentes científicas, su presencia en los índices y su relación con la [síntesis de fundamentos](topics/midnight-fundamentos-cientificos.md), la [entidad Midnight, NIGHT y DUST](entities/midnight-night-dust.md) y el [modelo token-recurso](concepts/modelo-token-recurso.md).
- Añadidas referencias recíprocas entre las páginas de fundamentos y de seguimiento de mercado, y entre las dos páginas complementarias de Midnight.
- Actualizada la referencia anterior que indicaba que no había publicaciones originales de Midnight archivadas: ahora existen documentos oficiales de arquitectura y tokenomics; siguen pendientes los anuncios originales y las métricas correspondientes al informe de mercado.
- Conservados sin cambios los PDF, sus metadatos y las cifras históricas del informe. No se infiere una causa de mercado a partir de los resultados de investigación.
- Revisión de coherencia: comprobados los enlaces locales de las cinco páginas actualizadas; no se encontraron enlaces rotos.

## [2026-10-05] summarize | Resumen de los cinco trabajos en la página de Midnight

- Añadido un resumen breve en [Midnight / NIGHT](entities/midnight-night.md), basado en las cinco fichas de lectura existentes: Kachina, Blockchain Space Tokenization, Minotaur, Proof-of-Stake Sidechains y precios unidimensionales frente a multidimensionales.
- Cada aportación enlaza su ficha, que conserva la referencia al PDF original y sus límites. Añadidas las cinco fuentes a la cabecera de la página y actualizado su resumen en el índice general.
- La lectura conjunta distingue privacidad, seguridad e interoperabilidad y asignación de capacidad; se mantiene pendiente contrastar su correspondencia con la implementación actual de Midnight.
- No se han alterado fuentes de RAW ni añadido afirmaciones sobre precios o rentabilidad.
- Actualizado también el índice de entidades y comprobados los enlaces del resumen; no se encontraron enlaces rotos.

## [2026-10-05] research + ingest | Tres preguntas abiertas de la visión general

- Lote solicitado por el usuario: elaborados y conservados primero en RAW los informes de [implementación de Midnight](../raw/reports/2026-10-05-midnight-fundamentos-implementacion.md), [fuentes de mercado, adopción y uso](../raw/reports/2026-10-05-fuentes-mercado-adopcion-uso.md) y [conciliación de IBIT](../raw/reports/2026-10-05-ibit-conciliacion-flujos-etf.md). Corte de investigación: 09:35:56, Europe/Madrid. Son informes derivados elaborados para esta base, no publicaciones independientes.
- Archivados 14 archivos de los repositorios de Midnight con revisiones resueltas de node-1.0.300 y ledger-8.1.2; verificada su coincidencia exacta con los blobs de GitHub. El [manifiesto](../raw/repos/2026-10-05-midnight-implementacion/manifiesto.json) conserva procedencia y diferencia entre el commit del tag reemitido y el target de la ficha de release.
- Contraste técnico: correspondencias parciales con Kachina, DUST, partner chains y precios por recurso. Documentada la diferencia de AURA/GRANDPA frente a Minotaur PoW/PoS y la divergencia entre 20.000 bytes de escritura propuestos en la especificación y 50.000 del código inicial. No se consultaron parámetros vivos ni se realizó una auditoría de mainnet.
- Identificados proveedores, componentes y metodología para mercado y uso; no se descargaron series completas de adopción, precios u OI. Conservada esa laguna.
- Archivadas las filas de Farside de las sesiones del 1 y 2 de octubre y la exportación original de BlackRock, con huella verificada. IBIT del día 2 sigue ausente en Farside. La aproximación por NAV y participaciones se registra separada; su diferencia con la sesión anterior del proveedor impide presentarla como flujo definitivo. El agregado de 134,4 millones de USD conserva su estado provisional.
- Creadas tres fichas de fuentes y tres [informes de la wiki](reports/index.md), la [comparación técnica](comparisons/midnight-investigacion-e-implementacion.md), el concepto [métricas de uso y adopción](concepts/metricas-de-uso-y-adopcion.md) y la entidad [IBIT](entities/ishares-bitcoin-trust-ibit.md).
- Actualizadas las entidades Cardano, Midnight y Bitcoin, los conceptos de ETF y token-recurso, los temas científicos y de mercado, la visión general, el índice general y los índices de categorías. Corregidas referencias actuales que mantenían pendiente todo el contraste o la captura de datos de ETF; se conserva el historial de estados previos en este registro.
- Revisión de coherencia: comprobados 46 archivos Markdown de la wiki y las notas/informes nuevos de RAW, con 38 páginas de wiki; sin enlaces locales rotos ni páginas huérfanas. Sin cambios en las huellas de los originales anteriores de RAW y sin discrepancias en los siete PDF del manifiesto. Las columnas publicadas de Farside suman 102,7 y 31,7; el dato ausente se conserva vacío.

## [2026-10-05] organize | Imágenes e indicación de actualización del índice

- Creada [raw/images](../raw/images/README.md) por indicación del usuario para imágenes descargadas o necesarias para la wiki, con originales y procedencia. Registrada la convención en AGENTS.md; otros adjuntos continúan en assets. No se descargaron imágenes nuevas en esta operación.
- Añadida al índice una fecha y hora visibles de última actualización en Europe/Madrid: 5 de octubre de 2026, 09:52. La marca se mantiene al editar el índice; no crea por sí sola un mecanismo automático de actualización.

## [2026-10-05] visuals | Imágenes e iconos en el índice

- Descargados recursos oficiales de Cardano y Midnight y conservados sin cambios en RAW/images. Los logotipos de Midnight se obtuvieron del repositorio oficial de documentación en una revisión fija, tras respuestas limitadas del sitio web; sus blobs se verificaron. La ilustración de privacidad se distingue del logotipo y queda disponible como recurso.
- Añadidos logotipos al inicio del índice, las variantes de Midnight para fondos claros y oscuros e iconos Unicode para identificar las secciones. El Markdown declara tamaños de presentación para Obsidian sin alterar los SVG originales.
- Añadida la [ficha de recursos visuales](sources/2026-10-05-recursos-visuales-indice.md), con origen, fechas conocidas, huellas y límites; actualizado el índice de fuentes y la marca de actualización del índice general a 5 de octubre de 2026, 10:02, Europe/Madrid.
- Revisión final: enlaces locales e imágenes válidos, sin nuevas páginas huérfanas; cinco recursos originales con SHA-256 verificado y SVG legibles como XML. Se comprobó la sintaxis de tamaños en la documentación oficial de Obsidian; no se certifica el renderizado de cada editor Markdown.

## [2026-10-05] presentation | Igualar el tamaño de los logotipos del índice

- Ajustada la presentación de Cardano y Midnight a una altura común de 40 píxeles, con anchos aproximados de 198 y 178 según las proporciones originales. Se usa HTML de presentación en el Markdown para expresar dimensiones explícitas.
- La variante de Midnight se selecciona según el fondo claro u oscuro mediante picture, evitando presentar dos logotipos simultáneamente. Los SVG originales y sus huellas se conservan sin cambios.
- Renovada la marca del índice a 5 de octubre de 2026, 10:05, Europe/Madrid.
- Ajuste final: altura común y ancho automático para conservar exactamente la proporción; referencias y huellas de originales comprobadas. La marca del índice queda en 5 de octubre de 2026, 10:07, Europe/Madrid.

## [2026-10-05] fix | Presentación de los logotipos con Markdown estándar

- El usuario informó de que los logotipos no aparecían en Codex tras introducir HTML. Una captura de la pantalla actual sí confirmó ambos logotipos con altura similar en Obsidian; no se pudo inspeccionar visualmente el panel de Codex.
- Sustituido el bloque HTML del [índice](index.md) por enlaces de imagen Markdown a copias PNG. Cada logo tiene 40 píxeles de altura y conserva sus proporciones dentro de un lienzo blanco de 220 × 64 píxeles; ya no depende de atributos HTML ni de sintaxis de tamaños específica de Obsidian.
- Conservados sin cambios los cinco recursos originales. Añadidas dos copias derivadas y sus [metadatos](../raw/images/2026-10-05-logotipos-indice-png-metadatos.json), con método, origen, dimensiones y SHA-256. Actualizadas la [ficha de recursos](sources/2026-10-05-recursos-visuales-indice.md) y la [convención de imágenes](../raw/images/README.md).
- Copias PNG inspeccionadas visualmente y dimensiones verificadas. Actualizada la marca del índice a 5 de octubre de 2026, 10:13, Europe/Madrid.
- Revisión final: 39 páginas de wiki sin enlaces locales rotos ni páginas huérfanas; siete imágenes con huellas verificadas. Una nueva captura confirmó la cabecera PNG visible en Obsidian. La marca del índice queda en 5 de octubre de 2026, 10:16, Europe/Madrid.

## [2026-10-05] verify | Cabecera visible en Codex

- La captura adjunta del usuario mostró que la versión HTML del índice se presentaba como texto en Codex. Tras sustituirla por las imágenes PNG enlazadas con Markdown, el usuario confirmó que veía los dos logotipos en su panel de Codex.

## [2026-10-05] version | Primera versión local en Git

- Por solicitud del usuario, incorporados los archivos del proyecto al control de versiones local: wiki, fuentes de RAW, imágenes, plantillas, documentos de referencia, instrucciones y configuración de Obsidian.
- Conservadas las exclusiones existentes: archivos temporales, .DS_Store y disposición de ventanas de Obsidian. El canvas existente se incluye en la versión inicial.
- El repositorio no tenía commits anteriores; esta operación registra la primera versión del proyecto.
