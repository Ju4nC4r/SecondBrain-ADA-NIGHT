---
title: "Migración de consenso y rotación de comités"
type: concept
created: "2026-10-27"
updated: "2026-10-27"
tags: [midnight, consenso, comites]
---

# Migración de consenso y rotación de comités

La [PR Midnight 2326](../sources/2026-10-27-midnight-transicion-consenso.md) ilustra un riesgo de coordinación: la inicialización de un nuevo mecanismo y la sustitución de autoridades en el mismo bloque pueden usar conjuntos distintos. La corrección descrita aplaza el cambio cuando corresponde rotación.

Una integración en main del repositorio demuestra estado del código; no una activación de red o transición completa. La descripción de pruebas tampoco equivale a reproducirlas. Versiones, parámetros, bloque de activación y observación efectiva de mainnet deben verificarse separadamente antes de afirmar consenso vigente.

Se conserva la [fotografía científica/técnica del 5](../reports/2026-10-05-midnight-fundamentos-implementacion.md) sin actualizarla por inferencia desde una PR. [Midnight](../entities/midnight-night.md) · [Versiones y despliegue](versiones-candidatas-y-despliegue.md) · [Índice](index.md).
