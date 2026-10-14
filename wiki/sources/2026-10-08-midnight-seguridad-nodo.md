# Midnight: contraste adicional del nodo 1.0.400

Fuentes primarias consultadas directamente: [notas del nodo](https://github.com/midnightntwrk/midnight-node/releases/tag/node-1.0.400) y [GHSA-wr7g-rr4v-jmj8](https://github.com/midnightntwrk/midnight-ledger/security/advisories/GHSA-wr7g-rr4v-jmj8). Consulta del 8, corte 07:20 Europe/Madrid; [notas](../../raw/notes/2026-10-08-fuentes-informe-diario.json). No se descargó código nuevo ni se reprodujo una prueba técnica.

- GitHub muestra release público **6 de octubre, 10:24**, sin zona explícita en el texto consultado. Las notas llevan fecha interna 5 y declaran el parche ya desplegado en Preview, Preprod y Mainnet, confirmado el **5**. Se distinguen publicación y despliegue; no hay instante exacto de este último.
- Nodo 1.0.400 incorpora ledger 8.1.3, corrección de una vulnerabilidad crítica. El aviso publicado el **1** indica afectación hasta 8.1.2 y versión corregida 8.1.3.
- La corrección de nuevas entradas no repara automáticamente estados afectados previamente guardados en contratos, según el aviso.

Es evidencia anterior recién incorporada al seguimiento, no un anuncio del día 8. El [contraste archivado del 5](../reports/2026-10-05-midnight-fundamentos-implementacion.md) se hizo contra revisiones fijadas 1.0.300 / 8.1.2; sigue siendo válido como fotografía histórica, no como representación del software actual. No se validan despliegue en vivo, explotación, pérdidas o estado de todos los contratos.

[Actualizaciones de seguridad](../concepts/actualizaciones-seguridad-midnight.md) · [Midnight](../entities/midnight-night.md) · [Informe del 8](../reports/2026-10-08-seguimiento-ada-night-bitcoin.md).
