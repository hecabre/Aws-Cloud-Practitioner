---
name: aws-cloud-practitioner-exams
description: Genera, guarda y califica exámenes de simulación en español de acuerdo con el temario construido desde las notas locales de este repositorio AWS Cloud Practitioner. Úsala para crear, practicar o calificar simulacros basados en esas notas; no la uses para exámenes sustentados principalmente en fuentes externas.
---

# Simulador AWS Cloud Practitioner

## Ubicar la bóveda

Esta es una skill del repositorio. Toma como raíz de la bóveda el ancestro que contiene `.agents/skills/aws-cloud-practitioner-exams` y usa:

- Notas fuente: `<raíz>/AWS Cloud Practitioner`
- Salida: `<raíz>/AWS Cloud Practitioner/Exámenes de simulación`

No dependas de una ruta absoluta ni de un nombre de usuario concreto.

## Fuente de verdad

Antes de generar preguntas, descubre y lee recursivamente los archivos Markdown de las notas fuente. Excluye `Exámenes de simulación`, `.obsidian`, `.trash` y cualquier examen o clave de respuestas ya generado.

Usa únicamente hechos que puedan justificarse con las notas. No completes vacíos con conocimiento general de AWS ni con Internet, salvo que el usuario pida explícitamente ampliar o verificar el contenido. Los enlaces de Obsidian, el texto visible y el destino enlazado forman parte de las notas.

Si el material no permite producir el número solicitado sin repetir o inventar, genera solamente la cantidad de preguntas únicas que admita y explica brevemente la limitación.

## Construir el temario

Antes de escribir el examen, construye un mapa del temario. Usa `Temario.md` como estructura principal y los archivos `Modulo N/00 - Modulo N.md` como índices de cada módulo. Completa esa estructura con las subcarpetas, encabezados y enlaces de las demás notas. Si esos índices no existen, usa `00 - Inicio.md`, sus secciones y sus wikilinks.

Identifica los temas principales, sus subtemas y las notas que los sustentan. Luego prepara internamente una distribución de preguntas de acuerdo con el temario:

- incluye cada tema principal cuando el número de preguntas lo permita;
- asigna más preguntas a los temas con más conceptos evaluables o mayor desarrollo en las notas;
- evita que una nota breve o repetitiva tenga el mismo peso que una unidad completa;
- considera `Resumen Rápido.md` como recapitulación de otros temas, no como una unidad independiente;
- si el usuario pide un tema, módulo o rango concreto, limita el temario y la distribución a ese alcance.

Resuelve expresiones como `Módulo 2`, `Modulo 2` o `2` contra la carpeta `Modulo 2`. Un módulo incluye recursivamente todas sus notas, pero excluye su archivo de índice como fuente de hechos cuando solo repita enlaces o descripciones del temario.

No conviertas los nombres de archivo en el temario sin revisar su contenido. La distribución debe representar lo estudiado, no solamente la cantidad de archivos.

## Generar un examen

Interpreta las preferencias expresas del usuario. Si no especifica alguna:

- Crea 20 preguntas, o menos si las notas no sostienen 20 preguntas distintas.
- Mezcla aproximadamente 75 % de selección única y 25 % de selección múltiple.
- Usa cuatro opciones por pregunta.
- Escribe todo en español.
- Distribuye las preguntas de acuerdo con el mapa del temario y la profundidad de cada tema.

Formula preguntas conceptuales y escenarios breves. En selección única debe existir una sola respuesta inequívoca. En selección múltiple indica cuántas opciones seleccionar y asegúrate de que exactamente esa cantidad sea correcta. Crea distractores plausibles mediante confusiones entre conceptos presentes en las notas o negaciones controladas; no introduzcas productos, límites, precios o propiedades ausentes de las fuentes.

Evita:

- preguntas duplicadas o meras paráfrasis dentro del mismo examen;
- pistas gramaticales, opciones absurdas y patrones obvios en la posición correcta;
- afirmaciones cuya validez dependa de información no escrita en las notas;
- copiar respuestas o explicaciones en el archivo que verá el estudiante.

## Guardar los archivos

Crea el directorio de salida si falta. Busca los archivos existentes para calcular el siguiente número correlativo de tres dígitos. Para el examen 7, por ejemplo, crea:

- `Examen 007.md`
- `Respuestas - Examen 007.md`

No sobrescribas archivos existentes. Si hay una colisión, incrementa el número.

El examen debe incluir:

```markdown
---
tipo: examen-simulacion
examen: 007
fecha: YYYY-MM-DD
estado: pendiente
preguntas: 20
---

# Examen de simulación 007

> Instrucciones: elige una opción, excepto cuando se indique “Selecciona dos”.

## Temario evaluado

- Tema principal
- Tema principal

## Pregunta 1

Texto de la pregunta

- [ ] A. Opción
- [ ] B. Opción
- [ ] C. Opción
- [ ] D. Opción

...

## Hoja de respuestas

1. ___
2. ___
```

No enlaces la clave desde el encabezado del examen ni reveles respuestas mediante comentarios, etiquetas o propiedades.

La clave separada debe incluir:

```markdown
---
tipo: clave-examen
examen: 007
fecha: YYYY-MM-DD
---

# Respuestas — Examen 007

## 1. B

Explicación breve de por qué es correcta y por qué el distractor más plausible no lo es.

**Fuente:** [[Nombre exacto de la nota]]

**Tema:** Nombre del tema del temario
```

Para una selección múltiple, registra todas las letras correctas. Cada explicación debe ser didáctica, concisa y citar al menos una nota mediante un wikilink válido. Si dos notas sostienen la respuesta, enlaza ambas.

Después de escribir los archivos, verifica:

- que el conteo declarado coincida con las preguntas reales;
- que todas las preguntas tengan cuatro opciones;
- que cada pregunta tenga respuesta y explicación;
- que los wikilinks de fuentes correspondan a notas existentes;
- que los temas y la distribución de preguntas correspondan al mapa del temario;
- que cada tema principal esté representado cuando el tamaño del examen lo permita;
- que la clave no sea necesaria para entender las instrucciones del examen;
- que ningún archivo previo haya sido modificado.

Al terminar, informa las rutas creadas, el número de preguntas y los temas cubiertos.

## Calificar una práctica

Cuando el usuario entregue sus respuestas, compáralas con la clave correspondiente. Acepta formatos compactos como `1B, 2AC, 3D`. Reporta aciertos, total, porcentaje y errores por tema; para cada error, da una explicación breve con wikilink a la nota que conviene repasar.

No cambies el examen ni la clave al calificar. Solo crea una nota de resultados si el usuario lo pide explícitamente.
