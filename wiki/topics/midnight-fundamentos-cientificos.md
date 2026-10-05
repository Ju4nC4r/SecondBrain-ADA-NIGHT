# Fundamentos científicos de Midnight y NIGHT

Actualizado: 2026-10-05. [Colección original y bibliografía](../../raw/articles/2026-10-05-midnight-bibliografia.md).

## Criterio de selección

Se priorizan los cinco trabajos que [IOG vincula al desarrollo de Midnight](https://www.iog.io/news/from-research-to-reality-building-midnight-on-peer-reviewed-foundations) y se añaden dos documentos oficiales para interpretar NIGHT y DUST. No se ha calculado un ranking por citas ni se afirma que la selección sea exhaustiva. La atribución de IOG es una declaración del desarrollador, no una evaluación independiente.

## Fuentes

- [Kachina - Foundations of Private Smart Contracts](../sources/kachina-foundations-private-smart-contracts.md): Base de contratos inteligentes privados y concurrencia.
- [Blockchain Space Tokenization](../sources/blockchain-space-tokenization.md): La relación científica más directa con el modelo de capacidad y costes NIGHT/DUST.
- [Minotaur: Multi-Resource Blockchain Consensus](../sources/minotaur-multi-resource-blockchain-consensus.md): Antecedente del consenso que combina recursos de seguridad.
- [Proof-of-Stake Sidechains](../sources/proof-of-stake-sidechains.md): Origen de la interoperabilidad segura y el merged staking en el recorrido de Midnight.
- [One-dimensional vs. Multi-dimensional Pricing in Blockchain Protocols](../sources/one-dimensional-vs-multi-dimensional-pricing.md): Estudia los costes y compromisos de valorar varios recursos de ejecución.
- [Midnight Tokenomics and Incentives Whitepaper](../sources/midnight-tokenomics-incentives.md): Documento principal para conocer la utilidad, oferta e incentivos del activo NIGHT.
- [Nightpaper: A litepaper introducing Midnight](../sources/midnight-nightpaper-litepaper.md): Introducción accesible a privacidad programable, arquitectura y NIGHT/DUST.

## Síntesis e interpretación

Las fuentes permiten estudiar tres capas: contratos privados (Kachina), seguridad e interoperabilidad (Minotaur y sidechains) y asignación de capacidad (BST y precios multidimensionales). Para el activo, el vínculo más directo es la [generación de DUST por NIGHT](../concepts/modelo-token-recurso.md), descrita en el whitepaper oficial.

Es una síntesis de lectura, no una prueba de que Midnight reproduzca todos los modelos originales. Tampoco convierte garantías de inclusión o incentivos en una predicción de rentabilidad.

## Diferencias entre fuentes y preguntas abiertas

El [Nightpaper](../sources/midnight-nightpaper-litepaper.md) denomina a NIGHT de política deflacionaria; el [whitepaper 1.81](../sources/midnight-tokenomics-incentives.md) distingue oferta total fija y expansión desinflacionaria de la oferta circulante por recompensas. Se conservan ambas formulaciones; para economía se prioriza la descripción detallada y versionada del whitepaper, sin reemplazar el original.

**Contraste añadido el 5 de octubre:** el [informe técnico](../reports/2026-10-05-midnight-fundamentos-implementacion.md) y la [comparación por mecanismo](../comparisons/midnight-investigacion-e-implementacion.md) identifican correspondencias parciales con código fijado del nodo y ledger. Minotaur no coincide con el consenso revisado; no se trasladan sus garantías al protocolo. Se conserva también una discrepancia entre especificación y código inicial de capacidad de escritura.

Falta comprobar parámetros y comité en un bloque finalizado de mainnet, la seguridad del puente y la equivalencia formal de las garantías. El [informe de fuentes y métricas](../reports/2026-10-05-fuentes-mercado-adopcion-uso.md) identifica cómo abordar la investigación empírica sobre demanda de uso, concentración y mercado; las series completas aún no se han obtenido.

[Midnight, NIGHT y DUST](../entities/midnight-night-dust.md) · [Modelo token-recurso](../concepts/modelo-token-recurso.md) · [Seguimiento de mercado de ADA y NIGHT](seguimiento-mercado-ada-night.md) · [Índice de temas](index.md).
