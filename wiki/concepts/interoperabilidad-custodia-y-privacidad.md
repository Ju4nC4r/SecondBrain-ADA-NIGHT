---
title: "Interoperabilidad: custodia, privacidad y disponibilidad"
type: concept
created: "2026-10-14"
updated: "2026-10-21"
tags: [cardano, midnight, defi, interoperabilidad, custodia]
sources:
  - "../sources/2026-10-21-informe-angry-crypto-show.md"
  - "../sources/2026-10-10-hoskinson-nightframes-tokio.md"
  - "../sources/2026-10-16-cardano-propuesta-cobre.md"
  - "../sources/2026-10-08-informe-angry-crypto-show.md"
  - "../sources/2026-10-09-informe-angry-crypto-show.md"
  - "../sources/2026-10-14-informe-angry-crypto-show.md"
---

# Interoperabilidad: custodia, privacidad y disponibilidad

Los casos del lote obligan a separar red, activo, ruta de ejecución, responsable de reservas y etapa de despliegue. Estas distinciones proceden de los informes archivados; no constituyen una auditoría nueva de sus implementaciones.

| Caso | Lo descrito en la fuente | Lo que no acredita |
|---|---|---|
| [Sundae v4, informe del 8](../sources/2026-10-08-informe-angry-crypto-show.md) | Enrutamiento y composición atómica entre pools | Intercambio entre cadenas o todos los ejemplos disponibles |
| [Minswap](../entities/minswap.md) | Hipótesis sobre Bitcoin/Midnight basada en encuesta e imágenes | Anuncio de integración o despliegue; negociar NIGHT en Cardano no es soportar la red Midnight |
| [Sig.Network](../entities/sig-network.md) | Descripción de firmas por umbral, demo en stagenet y roadmap | Mainnet ya comprobada o invisibilidad del tramo público de Ethereum |
| [Solada](../entities/solada.md) | Reservas bajo custodia y mercados con liquidez separada | Puente sin confianza, precios idénticos, reservas auditadas o adopción conseguida |

Una función prevista no equivale a una función ejecutada. Cada afirmación conserva su fuente, fecha y límite; condiciones de confianza, autenticación y visibilidad de cada tramo deben comprobarse antes de extraer garantías. [Infraestructura de acceso](infraestructura-de-acceso-a-la-red.md) · [Métricas de uso](metricas-de-uso-y-adopcion.md) · [Seguimiento del canal](../topics/seguimiento-angry-crypto-show.md).

## Revisión del 16 de octubre

La [propuesta de CuTT](../sources/2026-10-16-cardano-propuesta-cobre.md) prevé emisión en Ethereum y representación mediante puente en Cardano. Son componentes propuestos: no se convierten en un token ya operativo o reservas auditadas. Distinguir titularidad del cobre, custodia, saldo bloqueado y representación en otra red.

## Nightframes: propiedades pretendidas y pruebas pendientes

La [presentación original](../sources/2026-10-10-hoskinson-nightframes-tokio.md) propone no custodia, identidad, privacidad y ejecución demostrable para [Nightframes](nightframes.md). El ejemplo de pago sin conexión presupone que una clave no mantiene copias y puede borrarse de forma demostrable; no se aporta aquí un protocolo o hardware revisado que pruebe esas propiedades. Hablar de TEE, ZK y MPC no verifica automáticamente toda combinación o caso de uso.

Son distintos el control deseado del usuario, una wallet integrada declarada, la simulación pedagógica y el trading futuro en otras redes. Faltan atestaciones, modelo de amenazas, revocación/delegación y verificación de cada tramo; no se aplican garantías absolutas del discurso al estado vivo de Midnight.

## Revisión del 21 de octubre

[Nightmode, publicación oficial del 20](../sources/2026-10-21-midnight-nightmode.md), distingue activos nativos en bóvedas MPC de saldos representados privados; el tramo público expone importes. [Concepto relacionado](nightmode-privacidad-entre-redes.md). No se infiere privacidad absoluta, custodia auditada, implementación productiva o adopción de la descripción comercial. La nueva fuente complementa los antecedentes de SIG, sin reemplazarlos.

## Angry Crypto Show del 21: nativo, representación y tramo público

El [contraste recogido por el informe](../sources/2026-10-21-informe-angry-crypto-show.md) matiza «llevar tokens a Midnight»: activo nativo en origen, representación privada y cuentas controladas por firmantes umbral son componentes distintos. En Ethereum siguen visibles importes y tiempos. Stagenet y mainnet ligado a v9 no son disponibilidad universal, ni screening acredita cumplimiento en cualquier jurisdicción.

ADA→sUSDrf en SundaeSwap e iUSD/USDrf en Indigo PSM son rutas narradas sin ejecución o condiciones comprobadas. Canje nominal 1:1 y ausencia de deslizamiento no eliminan comisiones, insolvencia o límites de salida. [Liquidez](apr-credito-y-liquidez.md) · [Nightmode](nightmode-privacidad-entre-redes.md).
