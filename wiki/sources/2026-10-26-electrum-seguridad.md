---
title: "Electrum 4.8.3: aviso de servidor malicioso y RBF"
type: source
created: "2026-10-26"
updated: "2026-10-26"
tags: [bitcoin, electrum, seguridad]
---

# Electrum 4.8.3: aviso de servidor malicioso y RBF

[Aviso original GHSA-6jp4-8v48-cc5v](https://github.com/spesmilo/electrum/security/advisories/GHSA-6jp4-8v48-cc5v), SomberNight / Electrum, publicado 24 de octubre de 2026. [Notas de versión](https://raw.githubusercontent.com/spesmilo/electrum/master/RELEASE-NOTES), versión fechada 23. Leídos directamente el 25. [Fuentes y metadatos de consulta](../../raw/reports/2026-10-26-informe-ada-night-bitcoin-metadatos-publicacion.json). No artículo completo archivado.

Afectadas versiones <4.8.3; parche 4.8.3. El servidor puede ocultar un pago recién emitido y presentar otro inválido; al incrementar comisión mediante RBF el usuario puede firmar el pago al atacante. El proyecto declara explotación activa, dos informes privados (11 y 18) y pérdida en el segundo, importe no publicado. Etiqueta git del 23, binarios y divulgación del 24.

El parche verifica firmas de entradas propias en transacciones sin confirmar; no valida así todas las entradas ajenas ni convierte el cliente en nodo completo. El proyecto recomienda actualizar y comprobar direcciones/importes al firmar; no se ejecuta actualización de software del usuario. El aviso no demuestra vulneración del consenso Bitcoin o alcance total de pérdidas. [Electrum](../entities/electrum.md) · [Confianza y transacciones sin confirmar](../concepts/confianza-servidores-transacciones-sin-confirmar.md) · [BTC](../entities/bitcoin-btc.md) · [Informe](../reports/2026-10-26-seguimiento-ada-night-bitcoin.md).
