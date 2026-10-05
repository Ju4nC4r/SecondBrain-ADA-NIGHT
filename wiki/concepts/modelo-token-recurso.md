# Modelo token-recurso: NIGHT y DUST

Actualizado: 2026-10-05.

El [whitepaper oficial 1.81](../sources/midnight-tokenomics-incentives.md), secciones 2-3, separa un token transferible, NIGHT, de un recurso de ejecución, DUST. Para generar DUST se designa una dirección receptora; la tasa depende del saldo de NIGHT. DUST se consume y se degrada con el tiempo. Su no transferibilidad no impide acuerdos sobre la designación de generación futura.

[Blockchain Space Tokenization](../sources/blockchain-space-tokenization.md) estudia asignar derechos de uso de capacidad mediante tokens con garantías bajo un modelo adversarial. [Precios multidimensionales](../sources/one-dimensional-vs-multi-dimensional-pricing.md) estudia cómo valorar recursos distintos y señala compromisos entre eficiencia en equilibrio y transiciones.

Interpretación: ambos trabajos ayudan a razonar sobre costes de uso y congestión. No prueban por sí solos la implementación exacta de DUST ni un precio futuro del token.

**Contraste del 5 de octubre:** el [informe técnico](../reports/2026-10-05-midnight-fundamentos-implementacion.md) identifica en ledger 8.1.2 una capacidad inicial de 5 DUST por NIGHT, periodo de gracia de tres horas y un modelo de precios por dimensiones que se ajusta tras los bloques. Son constantes iniciales del código, no parámetros vigentes comprobados en mainnet. Tampoco se han acreditado las garantías de demora de BST para el mempool actual.

[Midnight, NIGHT y DUST](../entities/midnight-night-dust.md) · [Fundamentos científicos](../topics/midnight-fundamentos-cientificos.md) · [Índice de conceptos](index.md).
