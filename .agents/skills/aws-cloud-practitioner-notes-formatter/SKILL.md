---
name: aws-cloud-practitioner-notes-formatter
description: Mejora la estructura Markdown de las notas con cambios locales sin commit, o de un módulo, carpeta o nota indicada, en la bóveda AWS Cloud Practitioner para que sean más legibles y fáciles de estudiar, sin cambiar ni ampliar su significado técnico. Úsala al pedir formato, organización visual o mejor estructura de apuntes AWS; no la uses para verificar conceptos ni generar exámenes.
---

# Formato de notas AWS Cloud Practitioner

## Ubicar la bóveda

Esta es una skill del repositorio. Toma como raíz de la bóveda el ancestro que contiene `.agents/skills/aws-cloud-practitioner-notes-formatter` y usa `<raíz>/AWS Cloud Practitioner` como carpeta de notas. No dependas de una ruta absoluta ni de un nombre de usuario concreto.

El resultado debe facilitar la lectura, el repaso rápido y la relación entre conceptos, conservando exactamente la información y la intención del usuario.

## Delimitar el alcance

Usa Git para identificar archivos modificados, agregados, renombrados o sin seguimiento que todavía no pertenezcan a un commit. Considera cambios staged, unstaged y archivos untracked.

Por defecto, selecciona todos los `.md` con cambios locales dentro de la carpeta de notas. Excluye `.obsidian`, `.trash`, `Exámenes de simulación`, claves, resultados y archivos ajenos a las notas. Si no hay notas elegibles, informa que no hay nada que formatear y no modifiques archivos.

El usuario puede indicar un módulo, carpeta o nota. Una carpeta incluye sus Markdown recursivamente. Acepta rutas dentro de la bóveda, rutas relativas a la carpeta de notas, nombres con o sin `.md` y wikilinks. Resuelve `Módulo N`, `Modulo N` o el número aislado contra la carpeta canónica `Modulo N`. Intersecta siempre el objetivo con los archivos que tengan cambios locales sin commit. Si es ambiguo, pide que se precise antes de editar.

Antes de editar, lee completos los archivos seleccionados y revisa su estado y diff. En una nota nueva, revisa todo el contenido. Los cambios locales pertenecen al usuario: consérvalos y no restaures versiones anteriores.

## Qué mejorar

Adapta la estructura al contenido real; no impongas una plantilla idéntica. Cuando aporte claridad:

- usa un solo título `#` descriptivo y una jerarquía coherente de `##` y `###`, sin saltos de nivel;
- coloca una definición o idea central breve al inicio;
- divide bloques largos en secciones y párrafos cortos;
- convierte enumeraciones paralelas en listas y procesos secuenciales en listas numeradas;
- usa tablas sólo para comparaciones claras entre conceptos con las mismas dimensiones;
- resalta con negritas términos esenciales, no frases completas ni cada aparición;
- utiliza callouts de Obsidian con moderación para distinciones o advertencias importantes;
- agrupa enlaces bajo `## Relacionado` cuando ya cumplen esa función;
- normaliza espacios, líneas en blanco, indentación, viñetas y tablas.

Una nota breve y clara puede necesitar muy pocos cambios. Evita decoración, secciones vacías, tablas de una sola fila, exceso de callouts y fragmentar cada oración bajo un encabezado.

## Límites de contenido

Este flujo modifica presentación y organización, no conocimiento:

- no agregues, elimines ni corrijas afirmaciones técnicas;
- no cambies ejemplos, cifras, nombres de servicios o conclusiones;
- no consultes Internet; si detectas una posible imprecisión, repórtala y recomienda `$aws-cloud-practitioner-notes-polisher`;
- corrige errores mecánicos evidentes sólo cuando no alteren el significado;
- preserva frontmatter, código, embeds, imágenes, etiquetas, enlaces y wikilinks;
- no renombres ni muevas notas, ni cambies destinos de enlaces salvo para reparar sintaxis inequívocamente rota;
- no crees notas nuevas ni modifiques archivos fuera del objetivo;
- no hagas `git add`, commit ni push.

Si mejorar la estructura exigiría reescribir una idea ambigua, déjala intacta y señálala en el reporte.

## Verificar y entregar

Después de editar, relee cada nota y su diff; confirma que no se perdió ni añadió información, valida encabezados, listas, tablas, callouts y enlaces, y comprueba que sólo cambiaron los archivos seleccionados.

Informa en español las notas formateadas, las mejoras estructurales principales, cualquier ambigüedad que necesite `polish` y la confirmación de que no hiciste staging ni commit. Si una nota ya tenía buena estructura, no la cambies sólo para producir un diff.
