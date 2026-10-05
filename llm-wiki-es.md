# Wiki con LLM

Un modelo para construir bases de conocimiento personales con grandes modelos de lenguaje (LLM).

Este es un archivo de ideas, pensado para copiarlo y pegarlo en tu propio agente basado en un LLM, como OpenAI Codex, Claude Code, OpenCode / Pi u otros. Su objetivo es transmitir la idea general; tu agente desarrollará los detalles en colaboración contigo.

## La idea central

La experiencia de la mayoría de las personas con los LLM y los documentos se parece a la generación aumentada por recuperación (RAG): subes una colección de archivos, el LLM recupera los fragmentos pertinentes en el momento de la consulta y genera una respuesta. Esto funciona, pero el LLM vuelve a descubrir el conocimiento desde cero en cada pregunta. No hay acumulación. Plantea una pregunta sutil que requiera sintetizar cinco documentos y el LLM tendrá que encontrar y unir los fragmentos relevantes cada vez. No se construye nada que perdure. NotebookLM, la carga de archivos de ChatGPT y la mayoría de los sistemas RAG funcionan así.

Aquí la idea es diferente. En lugar de limitarse a recuperar información de los documentos originales en el momento de la consulta, el LLM **construye y mantiene progresivamente una wiki persistente**: una colección estructurada de archivos Markdown enlazados entre sí, situada entre tú y las fuentes originales. Cuando añades una fuente nueva, el LLM no se limita a indexarla para recuperarla más adelante. La lee, extrae la información clave y la integra en la wiki existente: actualiza páginas de entidades, revisa resúmenes de temas, señala dónde los datos nuevos contradicen afirmaciones anteriores y refuerza o cuestiona la síntesis en evolución. El conocimiento se compila una vez y después *se mantiene actualizado*, en lugar de volver a deducirse con cada consulta.

Esta es la diferencia fundamental: **la wiki es un resultado persistente cuyo valor se acumula.** Las referencias cruzadas ya están ahí. Las contradicciones ya se han señalado. La síntesis ya refleja todo lo que has leído. La wiki se enriquece con cada fuente que añades y cada pregunta que planteas.

Tú nunca, o casi nunca, escribes la wiki: el LLM la escribe y mantiene por completo. Tú te encargas de reunir las fuentes, explorar y hacer las preguntas adecuadas. El LLM realiza todo el trabajo laborioso: los resúmenes, las referencias cruzadas, el archivo y el registro que hacen que una base de conocimiento sea realmente útil a lo largo del tiempo. En la práctica, tengo el agente basado en un LLM abierto a un lado y Obsidian al otro. El LLM hace cambios a partir de nuestra conversación y yo exploro los resultados en tiempo real: sigo enlaces, compruebo la vista de grafo y leo las páginas actualizadas. Obsidian es el entorno de desarrollo; el LLM es el programador; la wiki es la base de código.

Esto puede aplicarse a muchos contextos diferentes. Algunos ejemplos:

- **Personal**: seguir tus propios objetivos, salud, psicología y desarrollo personal; archivar entradas de diario, artículos y notas de pódcast, e ir construyendo una imagen estructurada de ti mismo con el tiempo.
- **Investigación**: profundizar en un tema durante semanas o meses; leer trabajos académicos, artículos e informes, y construir progresivamente una wiki completa con una tesis en evolución.
- **Lectura de un libro**: archivar cada capítulo a medida que avanzas, crear páginas sobre personajes, temas, hilos argumentales y sus conexiones. Al terminar, tienes una wiki complementaria muy completa. Piensa en wikis de aficionados como [Tolkien Gateway](https://tolkiengateway.net/wiki/Main_Page): miles de páginas enlazadas entre sí sobre personajes, lugares, acontecimientos e idiomas, construidas por una comunidad de voluntarios a lo largo de los años. Podrías crear algo así para ti mientras lees, dejando al LLM todas las referencias cruzadas y el mantenimiento.
- **Empresa o equipo**: una wiki interna mantenida por LLM, alimentada con conversaciones de Slack, transcripciones de reuniones, documentos de proyectos y llamadas con clientes. Puede haber personas que revisen las actualizaciones. La wiki se mantiene al día porque el LLM realiza el mantenimiento que nadie del equipo quiere hacer.
- **Análisis de la competencia, diligencia debida, planificación de viajes, apuntes de cursos, profundización en aficiones**: cualquier actividad en la que acumules conocimiento con el tiempo y quieras tenerlo organizado en lugar de disperso.

## Arquitectura

Hay tres capas:

**Fuentes originales**: tu colección seleccionada de documentos fuente. Artículos, trabajos académicos, imágenes y archivos de datos. Son inmutables: el LLM los lee, pero nunca los modifica. Son tu fuente de verdad.

**La wiki**: un directorio de archivos Markdown generados por el LLM. Resúmenes, páginas de entidades, páginas de conceptos, comparaciones, una visión general y una síntesis. El LLM se encarga por completo de esta capa. Crea páginas, las actualiza cuando llegan fuentes nuevas, mantiene las referencias cruzadas y conserva la coherencia del conjunto. Tú la lees; el LLM la escribe.

**El esquema**: un documento, como CLAUDE.md para Claude Code o AGENTS.md para Codex, que indica al LLM cómo está estructurada la wiki, cuáles son las convenciones y qué flujos de trabajo debe seguir al incorporar fuentes, responder preguntas o mantener la wiki. Este es el archivo de configuración fundamental: lo que convierte al LLM en un mantenedor disciplinado de la wiki, en lugar de un chatbot genérico. Tú y el LLM vais desarrollándolo conjuntamente a medida que descubrís qué funciona para tu ámbito.

## Operaciones

**Incorporar fuentes.** Añades una fuente nueva a la colección de originales y pides al LLM que la procese. Un posible flujo: el LLM lee la fuente, comenta contigo las conclusiones principales, escribe una página de resumen en la wiki, actualiza el índice, actualiza las páginas de entidades y conceptos pertinentes y añade una entrada al registro. Una sola fuente puede afectar a entre 10 y 15 páginas de la wiki. Personalmente, prefiero incorporar las fuentes de una en una y seguir participando: leo los resúmenes, reviso las actualizaciones y oriento al LLM sobre qué aspectos destacar. Pero también puedes incorporar muchas fuentes por lotes, con menos supervisión. Tú decides qué flujo de trabajo encaja con tu estilo y lo documentas en el esquema para futuras sesiones.

**Consultar.** Haces preguntas sobre la wiki. El LLM busca páginas pertinentes, las lee y sintetiza una respuesta con citas. Las respuestas pueden adoptar diferentes formas según la pregunta: una página Markdown, una tabla comparativa, una presentación (Marp), un gráfico (matplotlib) o un lienzo. La idea importante es que **las buenas respuestas pueden incorporarse de nuevo a la wiki como páginas nuevas.** Una comparación que has pedido, un análisis o una conexión que has descubierto son valiosos y no deberían desaparecer en el historial del chat. Así, tus exploraciones se acumulan en la base de conocimiento del mismo modo que las fuentes incorporadas.

**Revisar la coherencia (lint).** Periódicamente, pide al LLM que compruebe el estado de la wiki. Busca contradicciones entre páginas, afirmaciones obsoletas que fuentes nuevas hayan dejado atrás, páginas huérfanas sin enlaces entrantes, conceptos importantes mencionados que no tengan su propia página, referencias cruzadas que falten y lagunas de información que puedan cubrirse con una búsqueda en la web. El LLM es bueno proponiendo preguntas nuevas que investigar y fuentes nuevas que buscar. Esto mantiene la wiki en buen estado a medida que crece.

## Indexación y registro

Dos archivos especiales ayudan al LLM, y a ti, a orientarse en la wiki a medida que crece. Cumplen funciones diferentes:

**index.md** está orientado al contenido. Es un catálogo de todo lo que hay en la wiki: cada página aparece con un enlace, un resumen de una línea y, opcionalmente, metadatos como la fecha o el número de fuentes. Se organiza por categorías: entidades, conceptos, fuentes, etc. El LLM lo actualiza cada vez que incorpora una fuente. Al responder una consulta, el LLM lee primero el índice para encontrar las páginas pertinentes y después profundiza en ellas. Esto funciona sorprendentemente bien a una escala moderada, con unas 100 fuentes y cientos de páginas, y evita la necesidad de una infraestructura RAG basada en representaciones vectoriales (embeddings).

**log.md** es cronológico. Es un registro al que solo se añaden entradas sobre lo que ocurrió y cuándo: incorporaciones de fuentes, consultas y revisiones de coherencia. Un consejo útil: si cada entrada empieza con un prefijo uniforme, por ejemplo `## [2026-04-02] ingest | Article Title`, el registro puede procesarse con herramientas sencillas de Unix; `grep "^## \[" log.md | tail -5` muestra las últimas cinco entradas. El registro ofrece una cronología de la evolución de la wiki y ayuda al LLM a entender qué se ha hecho recientemente.

## Opcional: herramientas de línea de comandos

En algún momento quizá quieras construir pequeñas herramientas que ayuden al LLM a trabajar con la wiki de forma más eficiente. La más evidente es un buscador para las páginas de la wiki: a pequeña escala basta con el archivo de índice, pero, cuando la wiki crece, necesitas una búsqueda adecuada. [qmd](https://github.com/tobi/qmd) es una buena opción: un buscador local para archivos Markdown que combina búsqueda BM25 y vectorial con reordenación de resultados mediante un LLM, todo en el propio dispositivo. Dispone tanto de una interfaz de línea de comandos, para que el LLM pueda ejecutarlo desde la consola, como de un servidor MCP, para que pueda usarlo como herramienta nativa. También podrías construir tú mismo algo más sencillo: el LLM puede ayudarte a programar mediante conversación un script de búsqueda básico cuando surja la necesidad.

## Consejos y trucos

- **Obsidian Web Clipper** es una extensión de navegador que convierte artículos web en Markdown. Resulta muy útil para incorporar rápidamente fuentes a tu colección de originales.
- **Descarga las imágenes localmente.** En la configuración de Obsidian, ve a «Files and links» y establece «Attachment folder path» en un directorio fijo, como `raw/assets/`. Después, en «Hotkeys», busca «Download», localiza «Download attachments for current file» y asígnale un atajo, por ejemplo Ctrl+Mayús+D. Tras capturar un artículo, pulsa el atajo y todas las imágenes se descargarán al disco local. Esto es opcional, pero útil: permite que el LLM vea las imágenes y haga referencia a ellas directamente, en lugar de depender de direcciones web que podrían dejar de funcionar. Ten en cuenta que los LLM no pueden leer de forma nativa el Markdown con imágenes insertadas en una sola pasada: la solución consiste en que el LLM lea primero el texto y después vea por separado algunas o todas las imágenes referenciadas para obtener más contexto. Es algo aparatoso, pero funciona razonablemente bien.
- **La vista de grafo de Obsidian** es la mejor forma de ver la estructura de tu wiki: qué está conectado con qué, qué páginas actúan como centros de conexión y cuáles están huérfanas.
- **Marp** es un formato de presentaciones basado en Markdown. Obsidian dispone de un complemento para utilizarlo. Es útil para generar presentaciones directamente a partir del contenido de la wiki.
- **Dataview** es un complemento de Obsidian que ejecuta consultas sobre los metadatos de cabecera de las páginas (frontmatter). Si tu LLM añade cabeceras YAML a las páginas de la wiki, con etiquetas, fechas y número de fuentes, Dataview puede generar tablas y listas dinámicas.
- La wiki no es más que un repositorio Git de archivos Markdown. Obtienes historial de versiones, ramas y colaboración sin trabajo adicional.

## Por qué funciona

La parte tediosa de mantener una base de conocimiento no es leer ni pensar, sino llevar los registros y mantener el orden. Actualizar referencias cruzadas, mantener los resúmenes al día, señalar cuándo los datos nuevos contradicen afirmaciones anteriores y conservar la coherencia entre decenas de páginas. Las personas abandonan las wikis porque la carga de mantenimiento crece más rápido que su valor. Los LLM no se aburren, no olvidan actualizar una referencia cruzada y pueden modificar 15 archivos en una sola pasada. La wiki se mantiene porque el coste de mantenimiento es prácticamente nulo.

El trabajo de la persona consiste en seleccionar las fuentes, orientar el análisis, hacer buenas preguntas y pensar en lo que significa todo ello. El trabajo del LLM es todo lo demás.

La idea está relacionada, en espíritu, con el Memex de Vannevar Bush (1945): un almacén de conocimiento personal y seleccionado, con recorridos asociativos entre documentos. La visión de Bush se parecía más a esto que a aquello en lo que acabó convirtiéndose la web: un sistema privado, organizado de forma activa, con conexiones entre documentos tan valiosas como los propios documentos. La parte que no pudo resolver era quién se encargaría del mantenimiento. El LLM se ocupa de eso.

## Nota

Este documento es deliberadamente abstracto. Describe la idea, no una implementación concreta. La estructura exacta de directorios, las convenciones del esquema, los formatos de página y las herramientas dependerán de tu ámbito, tus preferencias y el LLM que elijas. Todo lo mencionado es opcional y modular: elige lo que te resulte útil e ignora lo que no. Por ejemplo, tus fuentes podrían contener solo texto, de modo que no necesites gestionar imágenes. Tu wiki podría ser lo bastante pequeña como para que el archivo de índice sea suficiente y no haga falta un buscador. Puede que no te interesen las presentaciones y solo quieras páginas Markdown. O quizá prefieras un conjunto de formatos de salida completamente diferente. La forma adecuada de utilizar esta idea es compartirla con tu agente basado en un LLM y trabajar juntos para darle una forma que se ajuste a tus necesidades. La única función del documento es comunicar el modelo. Tu LLM puede resolver el resto.
