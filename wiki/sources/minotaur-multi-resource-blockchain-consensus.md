# Minotaur: Multi-Resource Blockchain Consensus

- Autoría: Matthias Fitzi; Xuechao Wang; Sreeram Kannan; Aggelos Kiayias; Nikos Leonardos; Pramod Viswanath; Gerui Wang.
- Tipo: Trabajo publicado en congreso con revisión por pares; copia de preprint.
- Publicación: 2022-11-07, ACM CCS 2022; DOI 10.1145/3548606.3559356.
- Versión: Copia arXiv 2201.11780v2, revisada 2022-09-07; primera entrega 2022-01-27. Se conserva el preprint, no el PDF editorial de ACM.
- Captura: 2026-10-05.
- [Fuente externa](https://arxiv.org/abs/2201.11780) · [PDF original](../../raw/articles/2026-10-05-minotaur-multi-resource-blockchain-consensus.pdf) · [Metadatos](../../raw/articles/2026-10-05-minotaur-multi-resource-blockchain-consensus-metadatos.md).

## Hechos y contenido de la fuente

Estudia un consenso que combina prueba de trabajo y prueba de participación. Los autores demuestran fungibilidad óptima de recursos bajo su modelo, generalizan el diseño y presentan un cliente en Rust con experimentos. Referencia: Resumen e introducción; PDF pp. 1-2.

## Relevancia para Midnight y NIGHT

Antecedente del consenso que combina recursos de seguridad. IOG incluye este trabajo en su [recorrido de investigación de Midnight](https://www.iog.io/news/from-research-to-reality-building-midnight-on-peer-reviewed-foundations).

## Límites e incertidumbres

No se infiere que Midnight ejecute hoy exactamente la combinación PoW/PoS del artículo; la correspondencia con el protocolo desplegado requiere documentación y código actuales. Esta ficha sintetiza las secciones indicadas; no constituye una revisión independiente de las demostraciones ni una auditoría del protocolo.

## Relaciones

- [Fundamentos científicos de Midnight](../topics/midnight-fundamentos-cientificos.md).
- [Midnight, NIGHT y DUST](../entities/midnight-night-dust.md).
- [Modelo token-recurso](../concepts/modelo-token-recurso.md).
