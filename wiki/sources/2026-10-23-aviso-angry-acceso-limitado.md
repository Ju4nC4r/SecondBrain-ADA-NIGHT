---
title: "Angry Crypto Show — aviso del 23: acceso limitado a dos vídeos"
type: source
created: "2026-10-23"
updated: "2026-10-23"
tags: [angry-crypto-show, acceso-limitado, pendiente, procedencia]
sources:
  - "../../raw/notes/2026-10-23-informe-angry-crypto-show.md"
  - "../../raw/notes/2026-10-23-informe-angry-crypto-show-metadatos.json"
---

# Angry Crypto Show — aviso del 23: acceso limitado a dos vídeos

## Original y naturaleza de la incorporación

[Aviso íntegro](../../raw/notes/2026-10-23-informe-angry-crypto-show.md) · [Metadatos, huellas y entrega](../../raw/notes/2026-10-23-informe-angry-crypto-show-metadatos.json) · [Infografía de estado](../../raw/images/2026-10-23-infografia-angry-crypto-show.png).

Es un **aviso de acceso limitado**, `report_type: access_limitation_notice`: registra dos publicaciones identificadas cuyo contenido sigue **pendiente de análisis**. Esta ingesta incorpora el aviso y su procedencia, no las noticias o recomendaciones de esos vídeos. No se crea una transcripción vacía o reconstruida ni se vuelve a analizar el episodio ya incorporado en la [edición del 21](2026-10-21-informe-angry-crypto-show.md).

## Publicaciones identificadas por el proceso de origen

El autor declara consulta directa del [canal, pestaña Vídeos recientes](https://www.youtube.com/@AngryCryptoShow/videos) y de los metadatos públicos, sin sesión/cookies. Al corte del **23 de octubre de 2026, 10:18 Europe/Madrid**, verifica canal, identificadores, títulos, fechas y duraciones. Esta incorporación comprueba los archivos archivados, sin volver a consultar YouTube o reproducir las descargas.

| Vídeo identificado | Publicación Europe/Madrid | Equivalencia UTC | Duración y estado |
|---|---|---|---|
| [qhIpkbPM_jc](https://www.youtube.com/watch?v=qhIpkbPM_jc) | **22 de octubre, 23:13:57** | 22 de octubre, 21:13:57 | Metadatos **12:23**; nuevo desde la revisión anterior, contenido no examinado. |
| [SCSBS7rDNKk](https://www.youtube.com/watch?v=SCSBS7rDNKk) | **22 de octubre, 00:20:46** | **21 de octubre, 22:20:46** | Metadatos **11:31**; tarjeta del canal observada el 22: **11:32**. Pendiente de la ejecución interrumpida del 22. |

Se conserva la discrepancia de un segundo sin resolverla por conjetura. La diferencia de fecha UTC/Madrid del segundo vídeo es conversión horaria, no otra publicación. Los títulos permanecen en los originales para identificar las fuentes; no se elevan a hechos, cifras, declaraciones comprobadas o recomendaciones.

## Acceso al contenido y lagunas

Ambos reproductores anunciaban pista inglesa automática (`asr`); las dos solicitudes públicas registraron **HTTP 200 y cero bytes**. Éxito del código HTTP no significa texto legible recuperado. Los metadatos declaran `transcript_status: not_available_in_this_run` y `transcript_path: null`.

No hay archivo de transcripción porque no se obtuvo texto legible; no se interpreta como ausencia universal de subtítulos en YouTube. Tampoco hay revisión íntegra de audio/gráficos, tramos de contenido verificados, noticias contrastadas o recomendaciones extraídas para estos dos episodios. Las declaraciones que pudieran contener siguen sin examinarse; las publicaciones verificadas no prueban sus titulares.

El aviso atribuye al proceso del 22 un rechazo de revisión automática al abrir YouTube mediante el conector de Brave, considerado ampliación de permisos al dominio, y no un rechazo manual del usuario. Declara no haber repetido o eludido esa acción; la consulta pública posterior sin sesión siguió sin aportar texto. Esta ingesta no intenta acceder al conector, cambiar permisos o superar el bloqueo. La petición de acceso que figura en el original es contexto histórico del proceso, no una autorización nueva.

## Ejecución interrumpida, entrega e ingesta separadas

- La ejecución del **22** quedó interrumpida según el aviso. En la búsqueda de Gmail descrita antes de preparar el del 23 no se halló una copia enviada con fecha editorial 22 ni 23. Esa observación es anterior a la entrega posterior registrada; no acredita ausencia global ni se afirma entrega del 22.
- **Preparación del aviso único del 23:** **10:21:51 Europe/Madrid**. Recoge un vídeo nuevo y otro pendiente, sin producir dos informes supuestamente analizados.
- **Envío del 23 registrado:** **10:25:52**; **verificación 10:26:36**; mensaje `1a167ddd3b85a910`, con imagen y cuerpo según metadatos del origen. Esta operación no accede a Gmail ni reenvía el aviso.
- **Archivo RAW:** **10:26:50**. **Ingesta local del aviso:** **23 de octubre**, posterior al archivo. Se conserva `ingestion_status: pending` en los metadatos originales como historia; la incorporación del aviso no cierra el análisis pendiente de los vídeos.

## Integridad y continuidad

Aviso e imagen coinciden en tamaños y SHA-256 con los metadatos. PNG **1024 × 1536** inspeccionado: dos vídeos pendientes, publicaciones del 22 en Madrid, horas resumidas a minutos y duraciones de metadatos; distingue texto vacío, audio no revisado y ausencia de inferencias desde títulos. «Verificado» corresponde a identificación/publicación según el proceso de origen, no a validación del contenido.

El seguimiento conserva **once análisis de vídeo y dos avisos de estado**: [revisión sin novedades del 19](2026-10-19-aviso-angry-sin-videos-nuevos.md) y este aviso de acceso limitado. Los dos vídeos actuales siguen pendientes, fuera del conjunto analizado. No se sustituye por ellos la serie diaria ADA/NIGHT/BTC ni sus lagunas.

[Registro elaborado de este aviso](../reports/2026-10-23-angry-crypto-show-acceso-limitado.md) · [Seguimiento del canal](../topics/seguimiento-angry-crypto-show.md) · [Índice de fuentes](index.md).
