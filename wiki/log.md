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

## [2026-10-05] verify | Publicación de la versión inicial en Gitea

- Verificado que `refs/heads/main` del remoto `origin` coincide con el commit local `a2f39fbd2aab231e1be27cacd5c2db0bbfd002f7`, tras la autenticación realizada por el usuario en la entrada oculta de Git.
- La excepción de comprobación TLS se limitó a las operaciones contra el repositorio indicado; no se guardó una desactivación global. Se conservaron los cambios de Obsidian y la eliminación del canvas fuera del commit inicial publicado.

## [2026-10-05] docs | README visual y guía de uso

- Reescrito el [README principal](../README.md) por solicitud del usuario: propósito, alcance, contenido existente, organización de RAW y wiki, incorporación de fuentes, consultas, revisión y control de versiones. Corregidas las referencias anteriores que aún indicaban ausencia de informes y de remoto.
- Añadidos iconos, los logotipos ya archivados, un árbol de carpetas y un [esquema del flujo](../docs/images/flujo-secondbrain.png), con su [original SVG](../docs/images/flujo-secondbrain.svg). La figura describe el proceso de trabajo; no representa un servicio automático nuevo.
- Incluido el inicio rápido de Obsidian: apertura de la raíz como bóveda existente, índice, enlaces a fuentes, búsqueda y grafo. Contrastados estos controles con la configuración local y la documentación oficial. Explicado el acceso por la pestaña Código de Gitea y la diferencia con su función Wiki separada.
- Verificación: 32 enlaces locales del README válidos, esquema SVG válido e imagen PNG inspeccionada visualmente. Los archivos preexistentes de Obsidian y la eliminación del canvas conservan su estado; no se han modificado originales de RAW.

## [2026-10-05] docs | Actualización de las instrucciones del proyecto

- Actualizado [AGENTS.md](../AGENTS.md) por solicitud del usuario con el nombre Second Brain ADA NIGHT, la identidad de los repositorios y el nombre conservado por la carpeta local.
- Registrada la configuración comprobada de Git: GitHub como remoto principal `origin`, Gitea como secundario `gitea` y seguimiento de `main` mediante `origin/main`. Corregidas en el [README](../README.md) las referencias que aún situaban Gitea como principal.
- Añadida la referencia a la [licencia Apache 2.0](../LICENSE), distinguiendo la licencia del proyecto de las licencias y atribuciones de fuentes y complementos de terceros. Conservadas las reglas existentes de organización, incorporación de fuentes y mantenimiento de la wiki.
- Verificación: 74 enlaces locales válidos en los tres documentos; configuración de remotos y seguimiento contrastada con Git. Las entradas históricas del registro y el texto de LICENSE se conservan sin cambios.

## [2026-10-06] ingest | Informe diario de ADA, NIGHT y Bitcoin

- Por solicitud del usuario, comprobados el chat «Informe diario de noticias de ADA y NIGHT» y el proyecto: no existía una entrega del día 6; se elaboró manualmente el [informe original](../raw/reports/2026-10-06-informe-ada-night-bitcoin.md), con corte documental a las 10:01 de Madrid, [metadatos y huellas](../raw/reports/2026-10-06-informe-ada-night-bitcoin-metadatos.md) y [notas de consulta](../raw/notes/2026-10-06-fuentes-informe-diario.json). Esta operación no acredita ni cambia la automatización.
- Incorporados el [informe diario](reports/2026-10-06-seguimiento-ada-night-bitcoin.md) y cuatro fichas: [procedencia](sources/2026-10-06-informe-ada-night-bitcoin.md), [Farside](sources/2026-10-06-farside-flujos-bitcoin.md), [estado del Cardano Summit](sources/2026-10-06-cardano-summit-estado.md) y [red y agenda de Midnight](sources/2026-10-06-midnight-red-y-agenda.md). Las notas conservan observaciones y metadatos, sin copiar íntegramente los artículos.
- Archivada una [nueva transcripción de doce fondos y tres sesiones](../raw/data/2026-10-06-farside-flujos-bitcoin.csv). IBIT del 2 de octubre ya figura en Farside; el agregado del 1–2 publicado asciende a 292,6 millones de USD. Se conserva el total provisional anterior y sigue abierta la discrepancia metodológica con NAV y participaciones del emisor.
- Contrastado el estado oficial del Summit con su planificación histórica. La cancelación no se presenta como anuncio del día 6 porque el aviso no está fechado. En Midnight se separan publicaciones anteriores, agenda futura y documentación operativa; no se infiere adopción ni se publica una cotización sin verificar.
- Actualizadas las páginas de Cardano, Midnight, Bitcoin e IBIT, los conceptos de flujos de ETF y métricas de uso, el seguimiento de mercado, la visión general y las referencias de los informes anteriores. Añadidos [gobernanza y tesorería](concepts/gobernanza-y-tesoreria.md) e [infraestructura de acceso](concepts/infraestructura-de-acceso-a-la-red.md), y mantenidos los índices general y de fuentes, informes, conceptos y entidades.
- Renovada la marca del índice al 6 de octubre de 2026, 10:05, Europe/Madrid. Los cambios preexistentes de Obsidian, docs/governance y pallets quedan fuera de la ingesta.
- Verificación: 46 páginas de wiki accesibles desde el índice, 548 referencias locales válidas y ninguna página huérfana. Comprobadas sumas de las tres filas de Farside, agregado del 1–2 y conversión de las horas de publicación; huellas de los nuevos originales válidas. Los 62 archivos anteriores de RAW y los cinco archivos ajenos registrados al inicio conservan sus huellas, y las entradas históricas del registro permanecen intactas.

## [2026-10-07] ingest | Informe diario de ADA, NIGHT y Bitcoin

- Elaborado manualmente el [informe completo](../raw/reports/2026-10-07-informe-ada-night-bitcoin.md), corte 07:50 Europe/Madrid, con [metadatos](../raw/reports/2026-10-07-informe-ada-night-bitcoin-metadatos.md) y [notas de consulta](../raw/notes/2026-10-07-fuentes-informe-diario.json). Comprobada ausencia de archivos del 7 antes de crear; los días anteriores no se duplican.
- Integrados [síntesis diaria](reports/2026-10-07-seguimiento-ada-night-bitcoin.md), [procedencia](sources/2026-10-07-informe-ada-night-bitcoin.md), [anuncio oficial de CIP-0113](sources/2026-10-07-cardano-tokens-programables.md) y [Farside](sources/2026-10-07-farside-flujos-bitcoin.md). Nuevo [concepto de tokens programables](concepts/tokens-programables-cip-0113.md).
- Nueva [fila CSV de ETF](../raw/data/2026-10-07-farside-flujos-bitcoin.csv), sesión del 6: total +118,8 millones de USD; suma verificada. Datos revisables y sin conciliación individual con emisores. Se conserva la discrepancia histórica de IBIT.
- Actualizados Cardano, Midnight, Bitcoin, IBIT, flujos de ETF, tema de seguimiento, visión general e índices general y de fuentes, informes y conceptos. Índices editados con marca 07:52 Europe/Madrid.
- Sin novedad fundamental de NIGHT identificada en las fuentes consultadas; evento posterior al corte, previamente conocido. Fechas de publicación ausentes declaradas. Sin cotizaciones simultáneas, comprobación independiente del código o cadena de CIP-0113 ni causalidad confirmada de precio. No se archivaron artículos completos.
- Verificación: 51 páginas de wiki accesibles desde el índice, 560 referencias locales válidas antes de añadir esta entrada, ninguna página huérfana; igualdad del cuerpo archivado con la entrega preparada. Los 66 archivos previos de RAW y 15 archivos ajenos conservan sus huellas. Historial de este registro intacto.
- No se modifican automatizaciones, horarios ni remotos; no se envían correos ni mensajes externos. La entrega manual no acredita ejecución automática satisfactoria.

## [2026-10-08] ingest | Informe diario de ADA, NIGHT y Bitcoin

- Elaboración por heartbeat diario, corte 07:20 Europe/Madrid. [Cuerpo completo](../raw/reports/2026-10-08-informe-ada-night-bitcoin.md), [metadatos y huella](../raw/reports/2026-10-08-informe-ada-night-bitcoin-metadatos.md) y [notas](../raw/notes/2026-10-08-fuentes-informe-diario.json). Comprobada ausencia de archivos del día antes de crear; no se duplican los anteriores.
- Incorporados [informe diario](reports/2026-10-08-seguimiento-ada-night-bitcoin.md), cinco fichas de fuentes, [Veridian](entities/veridian.md) y [actualizaciones de seguridad](concepts/actualizaciones-seguridad-midnight.md). Consulta primaria de comunicado de Cardano, release y aviso de Midnight y Farside. Productos de Midnight atribuidos a SIPO; post oficial bloqueado con 403.
- Separadas las fechas: Veridian anunciado el 8, productos atribuidos al 7, release del nodo publicado el 6 con despliegue declarado el 5 y aviso del 1. No se presenta el parche como anuncio nuevo del 8 ni se modifica la fotografía histórica de código. La búsqueda anterior de Midnight conservaba alcance limitado.
- Archivada la [fila de ETF de la sesión del 7](../raw/data/2026-10-08-farside-flujos-bitcoin.csv): doce fondos presentes, total −484,9 millones de USD, suma comprobada. Revisable y sin conciliación con emisores; persiste la discrepancia histórica de IBIT.
- Actualizadas entidades Cardano, Midnight, Bitcoin e IBIT, conceptos CIP-0113 y flujos de ETF, tema, visión general e índices general y de fuentes, entidades, conceptos e informes. Marca de actualización: 8 de octubre de 2026, 07:24 (Europe/Madrid).
- Verificación: 59 páginas de wiki accesibles desde el índice, 658 enlaces locales válidos antes de esta entrada (wiki y nuevos originales Markdown), ninguna página huérfana; cuerpo archivado idéntico a la entrega preparada y SHA-256 correcto. Los 70 archivos previos de RAW y 15 archivos ajenos conservan huellas; historial del registro intacto.
- Lagunas: emisión en cadena, post primario de productos y disponibilidad general, estado actual de nodos y contratos, explotación y escala de adopción sin comprobar. Sin cotizaciones simultáneas ni causalidad de precio; no se archivaron artículos completos.
- Verificada esta ejecución concreta del heartbeat y su archivo e integración. No se modifican programación ni remotos; no se envía correo ni mensajes externos.

## [2026-10-09] ingest | Informe diario de ADA, NIGHT y Bitcoin

- Elaborado por heartbeat el [informe completo](../raw/reports/2026-10-09-informe-ada-night-bitcoin.md), corte 08:56 Europe/Madrid, con [metadatos y huella](../raw/reports/2026-10-09-informe-ada-night-bitcoin-metadatos.md) y [notas de consulta](../raw/notes/2026-10-09-fuentes-informe-diario.json). Comprobada ausencia de archivos del 9 antes de crear. No se duplican los informes anteriores, incluido el del 5.
- Integrados [síntesis diaria](reports/2026-10-09-seguimiento-ada-night-bitcoin.md), [procedencia](sources/2026-10-09-informe-ada-night-bitcoin.md), [comunicado .ada](sources/2026-10-09-cardano-dominio-ada.md), [Farside](sources/2026-10-09-farside-flujos-bitcoin.md) y [mercado y liquidaciones](sources/2026-10-09-bitcoin-mercado-liquidaciones.md). Nuevos conceptos de [dominio e ICANN](concepts/dominio-ada-y-aprobacion-icann.md) y [liquidaciones](concepts/liquidaciones-posiciones-apalancadas.md).
- Separadas publicación del 8 e hito de ICANN del 7 atribuido a la Fundación; aprobación pendiente. Búsqueda de NIGHT sin novedad nueva confirmada, sin repetir los anuncios anteriores. Mercado del 8 descrito por CryptoSlate, no precio al corte; desgloses divergentes conservados y ventana CoinGlass no reconstruida. Un error transitorio de lectura externa se recuperó por una referencia previa; no se clasifica como enlace roto.
- Archivada [fila de doce fondos](../raw/data/2026-10-09-farside-flujos-bitcoin.csv), sesión del 8: −244,1 millones USD, suma comprobada. Con el 7, −729,0 por cálculo propio. Revisable, sin conciliación por emisor; discrepancia histórica de IBIT abierta.
- Actualizadas entidades Cardano, Midnight, Bitcoin e IBIT, flujos de ETF, tema de seguimiento, visión general e índices general y de fuentes, conceptos e informes. Marca de índices: 9 de octubre de 2026, 09:00 (Europe/Madrid).
- Verificación antes de esta entrada: 66 páginas accesibles desde el índice, 747 enlaces locales válidos (wiki y nuevos originales Markdown), ninguna página huérfana o enlace local roto. Cuerpo archivado idéntico al preparado para entrega; SHA-256 f4b0cad54379d0ec5f145e737e0c1718dc16456810983f3443093cd43531a545. Los 74 archivos previos de RAW y 15 archivos ajenos mantienen sus huellas. Historial del registro intacto.
- Lagunas registradas: lista ICANN independiente, aprobación y adopción, cifras compatibles de CoinGlass, conciliación por emisores y cobertura exhaustiva de redes sociales. Fuentes externas principales abiertas; sin auditoría completa de todos los enlaces externos históricos. No se archivaron artículos completos ni se confirma una causa única de precio.
- Comprobada esta ejecución concreta; no se modifican automatización, horarios ni remotos, ni se envían correos o mensajes externos. Bitcoin sigue como parte de los informes expresamente solicitados, sin ampliar el alcance general ADA/NIGHT.

## [2026-10-09] revise | Infografía para los informes diarios

- Solicitud del usuario: incluir una infografía a partir de ahora y volver a generar el informe de hoy. Creada y revisada visualmente con image_gen integrado; [imagen](../raw/images/2026-10-09-infografia-ada-night-bitcoin.png) y [prompt exacto y procedencia](../raw/images/2026-10-09-infografia-ada-night-bitcoin-metadatos.json).
- Añadida [revisión del informe con infografía](../raw/reports/2026-10-09-informe-ada-night-bitcoin-revision-con-infografia.md), con [metadatos propios](../raw/reports/2026-10-09-informe-ada-night-bitcoin-revision-con-infografia-metadatos.md). Texto factual y corte de 08:56 conservados. Original, metadatos y fuentes anteriores intactos; no se hace una segunda ingesta de las noticias ni se archivan artículos completos.
- Actualizadas síntesis diaria, ficha de procedencia del informe, visión general e índices general, de fuentes y de informes; nueva [ficha de imagen](sources/2026-10-09-infografia-informe-diario.md). Marca de índices: 9 de octubre de 2026, 09:47 (Europe/Madrid).
- Automatización noticias-diarias-de-ava actualizada mediante herramienta de Codex y comprobada en su configuración: infografía diaria incluida, estado ACTIVE y horario 07:00 Europe/Madrid conservados. No acredita futuras entregas.
- Verificación previa a esta entrada: 67 páginas wiki accesibles, 779 enlaces locales válidos, ninguna página huérfana ni enlace local roto. Cuerpo revisado equivale al anterior al retirar únicamente la referencia a imagen. SHA-256 de imagen e5504d3b3bebdf4b07ffb2f260197e37242751cb65e278624eeb6f04e93525fc; cuerpo revisado e56fac1f00b3fc7feeb56df47f5d436960bb5dca4d1db8b9f8b8d3d3ed57876e. Los 78 archivos previos de RAW y 15 archivos ajenos conservan huellas; historial de registro intacto. No commit, subida o envío externo.

## [2026-10-09] deliver | Informe diario por Gmail

- Envío autorizado expresamente por el usuario de cada informe terminado, con asunto antepuesto [Codex]. Automatización actualizada y comprobada: ACTIVE, horario diario 07:00 Europe/Madrid, informe completo e infografía a gallegojc@gmail.com, control de duplicados y constancia del envío.
- Enviado el informe de hoy por Gmail. Asunto: «[Codex] Informe diario de ADA, NIGHT y Bitcoin — 2026-10-09». Mensaje 1a11fa633bca4241, a gallegojc@gmail.com, fecha 2026-10-09T09:52:27+02:00. Respuesta de envío y lectura metadata con etiqueta SENT y encabezados correctos; no se afirma lectura por el destinatario.
- Conservada [nota nueva de envío](../raw/notes/2026-10-09-envio-gmail-informe-ada-night-bitcoin.json), con huellas del informe e imagen. Cuerpo HTML y texto, PNG inline. Se revisó Enviados para la misma fecha y asunto antes del envío.
- Actualizadas procedencia del informe, visión general e índices general, de fuentes y de informes. Marca 9 de octubre de 2026, 09:53 (Europe/Madrid). Los 82 archivos anteriores de RAW mantienen sus huellas; historial del registro conservado. No se reescriben hechos ni originales del informe.

## [2026-10-13] ingest | Informe diario con infografía

- Heartbeatdel13, corte07:58Europe/Madrid. [Cuerpoíntegro](../raw/reports/2026-10-13-informe-ada-night-bitcoin.md), [metadatos](../raw/reports/2026-10-13-informe-ada-night-bitcoin-metadatos.md), [notas](../raw/notes/2026-10-13-fuentes-informe-diario.json), [infografía](../raw/images/2026-10-13-infografia-ada-night-bitcoin.png) y [prompt yprocedencia](../raw/images/2026-10-13-infografia-ada-night-bitcoin-metadatos.json). No archivaartículoscompletos ni convierteinforme oimagenenfuentesprimarias.
- Incorporada [síntesisdiaria](reports/2026-10-13-seguimiento-ada-night-bitcoin.md) y cincofichas deprocedencia,gobernanza,OKJ,Farside ymercado. Reutilizadas entidadesCardano,Midnight,Bitcoin eIBIT yconceptosgobernanza,ETF yliquidaciones;actualizadosseguimiento,overview eíndicesgeneral,fuentes,informes,conceptos yentidades.
- SIPOreportadospropuestasexpiradas:fuentesprimariasAdaStatinaccesibles,resultadosatribuidos. DiferenciadasfechaJST12 yMadrid11 a23:44. OKJcontrastado directamenteencomunicadodelaempresadistribuidoenPRTIMES:inicio13 a10:00Madrid,futuroalcorte;no seafirmaapertura. PrecioBTCa03:20Madridypublicación03:57/actualización04:23,conversionesverificadas.
- [FilaETFdel12](../raw/data/2026-10-13-farside-flujos-bitcoin.csv):docecolumnaspresentes,suma-65,4millonesUSDcoincideconIBIT,revisableysinconciliaciónconemisores. Mercado yCoinGlassatribuidos aTheBlock;sinventanaoriginalreconstruida,nicausalidadúnica.
- No se localizaroncopiasdel10–12enlascarpetasconsultadasal inicio;lagunadearchivo,sininventarcausas oentregasretrospectivas. Últimoinformeconservado9. Noseduplicaninformesanteriores,incluido5.
- Verificación: 73páginaswikialcanzables,861enlaceslocalesválidosantesdeestaentrada,0huérfanas oenlaceslocalesrotos. SHA-256informe 48c24292f13d85eb1df8d8ef4925257b5492abb271d71299b8c0a2264f6e451e; imagen 1dbe88f424eaf3e15ac098fc0d567d4c4ce4dace3d4b0ed3ba14f2172e84c0d2. 83archivosanterioresdeRAWy15ajenosmantienenhuellas;historiadelregistrointacto. Texto eimagenvisualmentecontrastados. Marcadeíndices 13 de octubre de 2026, 08:04 (Europe/Madrid).
- Enlacesexternosmaterialesconsultados;fallosAdaStatysoporteOKJregistrados,sin declararrotura definitiva. Sin auditoríatotaldeenlacesexternoshistóricos. No se cambianhorarios,automatización oremotos. EnvíodeGmailse verificaráyregistraráenunanotanueva.

## [2026-10-13] deliver | Envío del informe por Gmail

- Enviado a gallegojc@gmail.com con asunto «[Codex] Informe diario de ADA, NIGHT y Bitcoin — 2026-10-13», a las 2026-10-13T08:10:08+02:00. Mensaje 1a133e1f5f7e22d5. Comprobados etiqueta SENT y encabezados To/Subject mediante respuesta de envío y lectura metadata. No se afirma lectura por el destinatario.
- [Nota de envío](../raw/notes/2026-10-13-envio-gmail-informe-ada-night-bitcoin.json) con fecha y huellas de cuerpo e imagen. HTML y texto completos, fuentes enlazadas e infografía PNG inline. Enviados revisado inmediatamente antes de enviar: no había mensaje de la misma fecha y asunto.
- Registrados el envío en procedencia, visión general e índices. Mejorado el espaciado de la prosa derivada del día para su lectura; no cambian hechos, referencias ni el cuerpo original en RAW. El registro de ingesta anterior permanece intacto.
- Los 89 originales anteriores de RAW conservan sus huellas. Se conserva el historial del registro. Sin cambios de horario, remotos o automatización.

## [2026-10-14] ingest | Informe diario ejecutado manualmente

- Petición expresa de ejecutar el informe pendiente del 14, recibida desde el chat coordinador. Ausencia de archivos y mensaje de fecha/asunto comprobada antes de crear; programación y estado ACTIVE conservados.
- Archivados [cuerpo completo](../raw/reports/2026-10-14-informe-ada-night-bitcoin.md), [metadatos](../raw/reports/2026-10-14-informe-ada-night-bitcoin-metadatos.md), [notas](../raw/notes/2026-10-14-fuentes-informe-diario.json), [fila ETF](../raw/data/2026-10-14-farside-flujos-bitcoin.csv), [infografía](../raw/images/2026-10-14-infografia-ada-night-bitcoin.png) y [prompt y procedencia](../raw/images/2026-10-14-infografia-ada-night-bitcoin-metadatos.json). Corte 08:35 Europe/Madrid. Informe e imagen derivados, no fuentes primarias; no artículos completos.
- Incorporadas cinco fichas de fuentes, síntesis diaria y conceptos [Leios: testnet y mainnet](concepts/leios-testnet-y-mainnet.md) y [roadmap y staking](concepts/roadmap-midnight-y-staking-night.md). Reutilizadas entidades Cardano, Midnight, BTC e IBIT y conceptos de ETF, métricas y modelo token-recurso; actualizados tema, overview e índices general, fuentes, informes, conceptos y entidades.
- Contenido primario contrastado en Musashi, release GitHub, roadmap Midnight, Farside y 8-K de Strive. Fechas de difusión atribuidas a SIPO porque X no se pudo leer. Planes futuros y estado histórico AURA/GRANDPA conservados; sin reinterpretar BABE previsto como despliegue actual o Minotaur.
- Farside, sesión del 13: doce columnas, suma +175,7 millones de USD verificada. Strive, anuncio del 13, compras del 5–9: 3.311 BTC, promedio 84.500 USD, saldo 32.773. Ventanas distintas, sin sumar como demanda simultánea o causa de precio.
- Verificación previa al registro: 81 páginas wiki alcanzables, 965 enlaces locales válidos, ninguna huérfana o enlace local roto. 90 originales previos RAW y 15 archivos ajenos conservan SHA-256; historial del registro intacto. Cuerpo archivado igual al preparado; huella c959e2af61fe5dccdd61d049fc691defb8b31fa648fa48599582c7e9b0cfe2d3, imagen 093f00c8f82c849d400696cdc38036b9fba2e20dc7692fb3dff47b3073b5f30f. Marca de índices 14 de octubre de 2026, 08:48 (Europe/Madrid).
- Lagunas: fechas de páginas oficiales, estado de ejecución y condiciones del staking, métricas de rendimiento propias, custodia y conciliación por emisores. Enlaces externos materiales consultados; no auditoría global histórica. El envío se verificará por lectura de cuerpo e imagen en Gmail y se registrará en nota nueva.

## [2026-10-14] deliver | Envío manual comprobado

- Enviado el informe terminado y su infografía por Gmail a gallegojc@gmail.com. Asunto: «[Codex] Informe diario de ADA, NIGHT y Bitcoin — 2026-10-14». Fecha 2026-10-14T08:50:43+02:00, mensaje 1a1392d79b3e05e4. Enviados revisado inmediatamente antes: sin duplicado de fecha/asunto.
- Leído el mensaje en formato full: SENT, destinatario y asunto correctos; cuerpos HTML y texto coinciden exactamente con los preparados. PNG inline recuperado mediante read_attachment y comprobado en memoria: 1542415 bytes, SHA-256 093f00c8f82c849d400696cdc38036b9fba2e20dc7692fb3dff47b3073b5f30f, idéntico al original. No se afirma lectura por el destinatario.
- Guardada [constancia de envío](../raw/notes/2026-10-14-envio-gmail-informe-ada-night-bitcoin.json), actualizadas procedencia, síntesis, overview e índices. Marca 14 de octubre de 2026, 08:53 (Europe/Madrid). Los 96 archivos previos de RAW conservan huellas; registro histórico intacto. Sin cambios o pausa de programación ni remotos.

## [2026-10-14] audit | Revisión de ingestas diarias del 6 al 14

- Por solicitud del usuario, revisado el lote de Noticias diarias ADA/NIGHT/BTC del 6–14, inclusive. Leído primero el índice, comprobados archivos, procedencia, páginas semánticas y el historial del chat origen hasta las entregas del 7 y comprobaciones del 6; examinadas también las salidas de la ejecución interrumpida del 10 y la carpeta de trabajo del chat. Otros seguimientos quedan fuera del alcance.
- Confirmados seis informes ya archivados e ingeridos: 6, 7, 8, 9, 13 y 14. Cada fecha tiene original y metadatos, ficha, síntesis, referencias en los cuatro activos, conceptos/tema, índices y una entrada de ingesta. No se encontró informe completo generado pendiente ni caso conservado solo en RAW; no se repiten ingestas.
- Lagunas 10–12: el historial muestra ejecución fallida del 10 con progreso pero sin cuerpo completo o entrega final recuperable. No se localizaron entregas completas separadas del 11–12 ni archivos del lote en la carpeta del chat. Se conserva el límite de la búsqueda y no se inventan informes retrospectivos.
- Comprobadas huellas declaradas de cuerpos y revisión del 9; el cuerpo de esa revisión, retirada la referencia de imagen, coincide con el original. Verificados PNG, dimensiones, huellas, vínculos e inspección visual de las infografías 9, 13 y 14. La nota original del 7 no declara SHA-256: se registra su huella actual sin modificarla; el texto noticioso coincide con la entrega revisada.
- Guardadas [evidencias nuevas](../raw/notes/2026-10-14-revision-ingestas-diarias-6-14.json) y [consulta de revisión](queries/2026-10-14-revision-ingesta-informes-6-14-octubre.md); actualizados visión general, índice de consultas e índice general. Marcas de índices: 14 de octubre de 2026, 09:44, Europe/Madrid. Los informes y fuentes anteriores permanecen intactos.
- La operación conserva los cambios ajenos y no hace commit, push, envíos o cambios de programación.
- Validación final acotada: 262 referencias locales válidas en los Markdown afectados; 82 páginas de wiki accesibles y ninguna huérfana. Los 97 originales anteriores de RAW y los 195 archivos previos fuera del alcance mantienen sus huellas; el prefijo histórico del registro permanece intacto. Continúa una sola entrada de ingesta por cada uno de los seis informes existentes y no se crean informes del 10–12.

## [2026-10-14] ingest | Lote de seis informes de Angry Crypto Show

- Petición del usuario trasladada desde «Informe Angry Crypto»: incorporar los seis informes archivados, además del lote ya comprobado de Noticias diarias ADA/NIGHT/BTC. Leídos AGENTS.md, índice, originales completos y metadatos; revisados segmentos pertinentes de las seis transcripciones automáticas. No se afirma una nueva revisión íntegra de audio o gráficos ni una nueva consulta primaria de todos los enlaces externos.
- [Manifiesto e índice originales](sources/2026-10-14-lote-angry-crypto-show.md): 24 archivos, con 23 huellas declaradas y el manifiesto conservado en la captura de integridad. Seis informes de revisión del 7, 8, 9, 10, 13 y 14; seis fichas de procedencia y seis síntesis creadas, con cuatro infografías originales enlazadas. No había páginas anteriores de ese canal que duplicar.
- Nuevas entidades Angry Crypto Show, Minswap, Solada y Sig.Network; conceptos de previsiones/publicidad e interoperabilidad/custodia; tema de seguimiento. Reutilizados Cardano, Midnight, Bitcoin, métricas, Leios, CIP-0113, roadmap y ficha primaria de Strive. Actualizados overview e índices general, fuentes, informes, entidades, conceptos y temas; marca 14 de octubre de 2026, 10:10 (Europe/Madrid).
- Preservadas atribuciones, incertidumbres de subtítulos, métricas no reproducidas, fases de testnet, disponibilidad futura y patrocino declarado de Kalshi. El cambio de afirmación sobre OKJ no acredita operación. Solada matiza liquidez unificada; los objetivos de Sheldon del 14 no heredan la entrada del 9. El contraste primario ya existente de Strive complementa la limitación secundaria del informe del canal, sin duplicar compras.
- Fechas del informe del 10 conservadas: revisión iniciada el 10, preparación e imagen el 12, envío efectivo el 13; la imagen no se corrige ni se reinterpreta como fecha de envío. No constan informes del canal del 1–6 ni del 11–12; no se infiere ausencia de vídeos ni se cubren lagunas de otra serie.
- Los originales RAW y metadatos de archivo permanecen intactos, incluido el estado histórico pending del manifiesto. La incorporación posterior se registra aquí. No se hacen commits, subidas, reenvíos o cambios de programación desde este chat; la publicación autorizada se coordina en «Informe Angry Crypto».
- Validación final: 102 páginas de wiki accesibles, 1.427 referencias locales válidas y ninguna página huérfana. Seis fichas y seis síntesis, cuatro PNG verificados y enlazados; fechas del informe del 10 explícitas. Los 122 originales previos de RAW y los archivos ajenos mantienen sus huellas; el prefijo histórico del registro está intacto. Las 25 notas de raw/notes están referenciadas: seis informes sustantivos del canal ya ingeridos y 19 archivos de procedencia, metadatos, entrega o auditoría que no requieren página conceptual propia.
