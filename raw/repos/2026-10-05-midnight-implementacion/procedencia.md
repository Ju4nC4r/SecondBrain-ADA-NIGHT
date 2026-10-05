# Captura de repositorios Midnight

Captura: 5 de octubre de 2026, 09:35:56, Europe/Madrid.

Los archivos de `node/` y `ledger/` conservan el contenido obtenido mediante la API de GitHub, sin ejecutar ni modificar el código. El [manifiesto](manifiesto.json) identifica repositorio, ruta, blob y revisión fija de cada archivo. Las versiones se eligieron contrastando las [notas oficiales del nodo](https://docs.midnight.network/relnotes/node) y la dependencia exacta de Cargo.toml.

La fecha de captura no es la fecha de publicación de cada archivo. Para publicación y cambios debe consultarse el historial de su revisión. La etiqueta de nodo fue reemitida: se conserva el commit resuelto del tag y también el target de la ficha de release, que difieren. No se ha consultado el estado RPC de mainnet ni confirmado el binario que ejecuta cada operador.

Uso: [informe de contraste](../../reports/2026-10-05-midnight-fundamentos-implementacion.md).

