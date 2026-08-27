---
name: aws-cloud-practitioner-notes-polisher
description: Audita y pule en español las notas Markdown de AWS Cloud Practitioner que tienen cambios locales sin commit dentro de un módulo, carpeta o nota, contrastándolas con el contexto de la bóveda y documentación oficial de AWS para detectar omisiones, conceptos confusos o interpretaciones incorrectas. Úsala al revisar apuntes AWS recientes; no la uses para generar exámenes ni para reescribir notas ya consolidadas.
---

# Pulido de notas AWS Cloud Practitioner

## Ubicar la bóveda

Esta es una skill del repositorio. Toma como raíz de la bóveda el ancestro que contiene `.agents/skills/aws-cloud-practitioner-notes-polisher` y usa `<raíz>/AWS Cloud Practitioner` como carpeta de notas. No dependas de una ruta absoluta ni de un nombre de usuario concreto.

El objetivo es dejar los apuntes recientes correctos, claros y útiles para estudiar, sin borrar la voz del usuario ni convertir cada nota en una referencia exhaustiva.

## Delimitar el alcance

Usa Git para identificar archivos modificados, agregados, renombrados o sin seguimiento que todavía no pertenezcan a un commit. Considera cambios staged, unstaged y archivos untracked.

Por defecto, procesa únicamente archivos `.md` con cambios locales dentro de la carpeta de notas. Excluye `.obsidian`, `.trash`, `Exámenes de simulación`, claves, resultados y archivos ajenos a las notas. Si no hay notas elegibles, informa que no hay nada que pulir y no modifiques archivos.

El usuario puede indicar un módulo, carpeta o nota. Una carpeta incluye sus Markdown recursivamente. Resuelve `Módulo N`, `Modulo N` o el número aislado contra la carpeta canónica `Modulo N`. Intersecta siempre el objetivo con los archivos que tengan cambios locales sin commit. Si el objetivo es ambiguo, pide que se precise antes de editar.

Antes de editar, revisa el diff completo de cada nota tracked; en una nota nueva, revisa todo el contenido. Los cambios locales pertenecen al usuario: consérvalos y no confundas cambios internos de Obsidian con apuntes académicos.

## Obtener contexto y evidencia

Para cada nota seleccionada:

1. Lee la versión de trabajo y, cuando exista en `HEAD`, compárala con la versión confirmada.
2. Lee las notas enlazadas o directamente relacionadas necesarias para conservar vocabulario, alcance y wikilinks. Usa `Temario.md`, el índice `Modulo N/00 - Modulo N.md` correspondiente y `00 - Inicio.md` como mapas.
3. Verifica las afirmaciones técnicas mediante fuentes oficiales y primarias de AWS, como AWS Documentation, AWS Whitepapers, AWS Skill Builder o páginas oficiales del servicio. Navega por Internet porque la documentación puede cambiar; no uses blogs de terceros para decidir una corrección.

No trates la memoria general del modelo como evidencia suficiente. Si una fuente oficial no resuelve una duda, conserva el texto cuando no sea claramente falso y registra la incertidumbre en el reporte.

## Criterios de revisión

Evalúa el material en cinco dimensiones:

- **Exactitud:** definiciones, relaciones, responsabilidades, condiciones y ejemplos correctos.
- **Comprensión:** distingue conceptos que suelen confundirse y corrige formulaciones engañosas.
- **Cobertura proporcional:** añade sólo conceptos esenciales para entender el tema que la nota intenta explicar.
- **Claridad:** español natural, ortografía y estructura que faciliten el estudio.
- **Integración:** wikilinks válidos, terminología coherente y ausencia de duplicación innecesaria.

Presta especial atención a absolutos como “siempre”, “todas”, “sólo” o “deja de generar costos”. Distingue una simplificación pedagógica aceptable de una afirmación técnicamente falsa.

## Aplicar el pulido

A menos que el usuario pida explícitamente una auditoría sin cambios, edita directamente las notas elegibles.

- Conserva la intención, el nivel de detalle y el estilo de la bóveda.
- Corrige errores claros y completa vacíos materiales con formulaciones concisas.
- En notas tracked, concentra el trabajo en los conceptos cambiados y el contexto mínimo necesario; en notas nuevas, pule la nota completa.
- Mantén los wikilinks y crea uno nuevo sólo si su destino ya existe o el usuario pidió crear también esa nota.
- No agregues bibliografías o URLs dentro de las notas salvo que se solicite; presenta las fuentes en el reporte final.
- No alteres notas relacionadas sólo para uniformarlas. Reporta aparte los problemas fuera del alcance.
- No añadas límites, precios o características volátiles sin respaldo oficial actual.
- No hagas `git add`, commit, push ni modifiques configuración de Obsidian.

Si el usuario pide sólo revisar, no edites: entrega hallazgos con severidad, ubicación y corrección propuesta.

## Verificar y entregar

Después del pulido, relee cada archivo y su diff; confirma que sólo cambiaron las notas seleccionadas, que los wikilinks nuevos existen y que no se perdieron ideas originales ni aparecieron contradicciones.

Resume en español las notas revisadas, las correcciones y omisiones completadas, lo que ya era correcto, las dudas o mejoras pendientes y los enlaces a fuentes oficiales. Confirma que no hiciste staging ni commit. No declares que una nota está completa en sentido absoluto; indica si cubre suficientemente su alcance.
