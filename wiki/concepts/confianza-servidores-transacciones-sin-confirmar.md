---
title: "Confianza en servidores y transacciones sin confirmar"
type: concept
created: "2026-10-26"
updated: "2026-10-26"
tags: [bitcoin, electrum, seguridad]
---

# Confianza en servidores y transacciones sin confirmar

El [caso Electrum](../sources/2026-10-26-electrum-seguridad.md) distingue información presentada por un servidor de una transacción confirmada y validada. Una sustitución inválida en el historial puede inducir una firma posterior válida al aumentar la comisión. Cambiar comisión es una firma con efectos, no una validación de que el destinatario anterior fuese correcto.

La versión 4.8.3 verifica firmas de entradas propias en transacciones mempool; no valida por esa vía todas las entradas ajenas o ancestros, y no es nodo completo. Preservar alcance del parche, versión y fecha antes de extrapolar a la seguridad de toda la red. [Electrum](../entities/electrum.md) · [BTC](../entities/bitcoin-btc.md) · [Versiones y despliegue](versiones-candidatas-y-despliegue.md) · [Índice](index.md).
