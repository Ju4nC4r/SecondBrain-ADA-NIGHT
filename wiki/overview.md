# Visión general

## Alcance

Base de conocimiento personal para investigar Cardano (ADA) y Midnight (NIGHT) con fuentes trazables y páginas enlazadas.

## Estado

La estructura conserva la [guía de Karpathy](sources/llm-wiki.md) y una [copia del informe de ADA, NIGHT y Bitcoin](sources/2026-10-05-informe-ada-night-bitcoin.md) del 5 de octubre, procedente de otro chat y guardada en RAW con sus metadatos. El informe ya está integrado en [una síntesis diaria](reports/2026-10-05-seguimiento-ada-night-bitcoin.md), páginas de activos, conceptos y un tema de seguimiento. Las cotizaciones y el interés abierto de esa primera fotografía siguen sin nueva verificación. La revisión posterior de ETF sí conserva datos de Farside y una exportación primaria de BlackRock, con los límites descritos abajo.

El 5 de octubre se incorporó la [bibliografía científica y técnica de Midnight](topics/midnight-fundamentos-cientificos.md): siete PDF originales, cinco trabajos publicados en congresos y dos documentos oficiales, con versiones y procedencia registradas.

También se elaboraron tres informes sobre las preguntas abiertas, conservados en RAW e incorporados con sus fichas de fuente: [implementación de Midnight](reports/2026-10-05-midnight-fundamentos-implementacion.md), [fuentes de mercado, adopción y uso](reports/2026-10-05-fuentes-mercado-adopcion-uso.md) y [conciliación de IBIT](reports/2026-10-05-ibit-conciliacion-flujos-etf.md). Se archivaron 14 archivos de código con revisiones fijadas, datos observados de Farside y la exportación original de BlackRock.

## Síntesis

El primer informe integrado describe un repunte de ADA, un retroceso de NIGHT y entradas provisionales en ETF de Bitcoin. Se conservan como afirmaciones de una fuente derivada, con fechas y atribución; no como una validación independiente de sus cifras o de las causas de los movimientos. La [síntesis de seguimiento](topics/seguimiento-mercado-ada-night.md) reúne las relaciones y lagunas.

RAW conserva el informe original. Las páginas de la wiki contienen su elaboración y referencias cruzadas, y el registro mantiene el historial de operaciones.

El contraste técnico identifica mecanismos relacionados con Kachina, DUST y precios por recurso. AURA/GRANDPA en el nodo revisado difiere de Minotaur PoW/PoS. Se documenta además una diferencia entre capacidad de escritura propuesta en la especificación y el código inicial; no se atribuyen esos parámetros al estado vivo. [Evidencia y límites](comparisons/midnight-investigacion-e-implementacion.md).

Las fuentes para estudiar mercado y uso están identificadas, pero faltan series empíricas completas. Farside aún deja ausente IBIT del 2 de octubre al corte de la revisión; el total de 134,4 millones de USD sigue provisional. Una aproximación con NAV y participaciones del emisor no concilia con la fecha o metodología del proveedor y se conserva separada.

La carpeta [RAW/images](../raw/images/README.md) conserva las imágenes descargadas o necesarias para la wiki, con procedencia y originales sin modificar.

## Flujo diario configurado

La automatización «Noticias diarias de ADA, NIGHT y Bitcoin» conserva la entrega en el chat «Informe diario de noticias de ADA y NIGHT» a las 07:00, Europe/Madrid. Desde el 5 de octubre incluye instrucciones para archivar cada informe en RAW e integrar su contenido en la wiki. Se ha verificado la configuración guardada; queda pendiente comprobar el primer guardado e integración realizados por una ejecución automática posterior.

## Preguntas abiertas

- Qué parámetros y comité muestra mainnet en un bloque finalizado y cómo se justifican las garantías científicas en la implementación; [contraste documental parcial completado](reports/2026-10-05-midnight-fundamentos-implementacion.md).
- Qué resultados aportan series históricas completas de mercado, adopción y uso; [fuentes y método identificados](reports/2026-10-05-fuentes-mercado-adopcion-uso.md), descarga y análisis empírico pendientes.
- Cómo conciliar fechas y metodología del flujo de IBIT y obtener el dato diario publicado; [estado pendiente comprobado y fuentes archivadas](reports/2026-10-05-ibit-conciliacion-flujos-etf.md), sin convertir el total provisional en definitivo.
