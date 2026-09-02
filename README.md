# AWS Cloud Practitioner

Notas de estudio en español para preparar la certificación **AWS Certified Cloud Practitioner**. El repositorio está organizado como una bóveda de [Obsidian](https://obsidian.md/) y conecta los conceptos mediante enlaces internos para facilitar el repaso.

## Contenido

Actualmente, las notas cubren los primeros cuatro módulos del curso:

- **Módulo 1 — Introducción a Amazon Web Services:** fundamentos de la nube, modelo cliente-servidor y responsabilidad compartida.
- **Módulo 2 — Cómputo e infraestructura de AWS:** Amazon EC2, AMI, virtualización, tipos de instancias, precios, tenencia, regiones y zonas de disponibilidad.
- **Módulo 3 — Servicios de cómputo y aplicaciones modernas:** contenedores, servicios administrados, AWS Lambda, AWS Batch, AWS Elastic Beanstalk, AWS Fargate, AWS Outposts y Amazon Lightsail.
- **Módulo 4 — Infraestructura global y automatización:** regiones, alta disponibilidad, red de borde, Amazon CloudFront, infraestructura como código y AWS CloudFormation.
- Un resumen rápido para el repaso final.

## Cómo usar este repositorio

### Con Obsidian

1. Clona el repositorio:

   ```bash
   git clone https://github.com/hecabre/Aws-Cloud-Practitioner.git
   ```

2. Abre Obsidian y selecciona **Abrir carpeta como bóveda**.
3. Elige la carpeta raíz del repositorio.
4. Empieza por la nota [00 - Inicio](AWS%20Cloud%20Practitioner/00%20-%20Inicio.md) y continúa con el [Temario](AWS%20Cloud%20Practitioner/Temario.md).

Obsidian resolverá los enlaces internos con formato `[[Nombre de la nota]]` y permitirá explorar las relaciones entre temas mediante su vista de grafo.

### Desde GitHub

También puedes leer las notas directamente en GitHub. Usa [00 - Inicio](AWS%20Cloud%20Practitioner/00%20-%20Inicio.md) como índice principal y continúa con el [Resumen Rápido](AWS%20Cloud%20Practitioner/Resumen%20Rápido.md) para repasar los puntos clave.

> GitHub muestra los enlaces internos de Obsidian como texto, pero los enlaces Markdown de este README sí permiten acceder a las notas principales.

## Estructura

```text
.
├── .agents/skills/                  # Skills locales para exámenes y notas
├── .obsidian/                       # Configuración de la bóveda
├── AWS Cloud Practitioner/
│   ├── 00 - Inicio.md               # Índice principal
│   ├── Temario.md                     # Programa e índices por módulo
│   ├── Modulo 1/                     # Introducción a AWS
│   ├── Modulo 2/                     # EC2 e infraestructura de AWS
│   │   └── Tipos de Instancias/      # Detalle de cada familia EC2
│   ├── Modulo 3/                     # Cómputo y aplicaciones modernas
│   ├── Modulo 4/                     # Infraestructura global y automatización
│   └── Resumen Rápido.md
└── README.md
```

## Ruta de estudio sugerida

1. [Módulo 1 — Introducción a Amazon Web Services](AWS%20Cloud%20Practitioner/Modulo%201/00%20-%20Modulo%201.md)
2. [Módulo 2 — Cómputo e infraestructura de AWS](AWS%20Cloud%20Practitioner/Modulo%202/00%20-%20Modulo%202.md)
3. [Módulo 3 — Servicios de cómputo y aplicaciones modernas](AWS%20Cloud%20Practitioner/Modulo%203/)
4. [Módulo 4 — Infraestructura global y automatización](AWS%20Cloud%20Practitioner/Modulo%204/00%20-%20Modulo%204.md)
5. [Resumen Rápido](AWS%20Cloud%20Practitioner/Resumen%20R%C3%A1pido.md)

## Skills de Codex

El repositorio incluye tres skills que Codex detecta automáticamente al trabajar dentro de la bóveda:

- [`aws-cloud-practitioner-exams`](.agents/skills/aws-cloud-practitioner-exams/SKILL.md): genera y califica simulacros basados únicamente en las notas.
- [`aws-cloud-practitioner-notes-polisher`](.agents/skills/aws-cloud-practitioner-notes-polisher/SKILL.md): contrasta apuntes recientes con documentación oficial de AWS y corrige errores u omisiones materiales.
- [`aws-cloud-practitioner-notes-formatter`](.agents/skills/aws-cloud-practitioner-notes-formatter/SKILL.md): mejora la estructura Markdown sin cambiar el significado técnico.

### Generar un examen

```text
Usa $aws-cloud-practitioner-exams para crear un examen de simulación basado en mis notas.
```

La skill usa `Temario.md` y los índices de módulo para distribuir las preguntas, genera el examen y su clave en archivos separados, y también permite limitar un simulacro a un módulo concreto. Los simulacros se guardan en `AWS Cloud Practitioner/Exámenes de simulación/`.

### Pulir notas recientes

```text
Usa $aws-cloud-practitioner-notes-polisher para revisar y pulir las notas sin commit del Módulo 2.
```

`polish` verifica conceptos con fuentes oficiales actuales de AWS, conserva el alcance de los apuntes y no hace staging, commit ni push.

### Mejorar el formato

```text
Usa $aws-cloud-practitioner-notes-formatter para mejorar la estructura Markdown de las notas sin commit del Módulo 2.
```

`format` sólo reorganiza la presentación del contenido: no verifica ni amplía afirmaciones técnicas y tampoco ejecuta operaciones de Git.

## Contribuciones

Las mejoras, correcciones y nuevas notas son bienvenidas. Para mantener la bóveda consistente:

- Usa Markdown para el contenido.
- Escribe nombres de archivo descriptivos.
- Conecta las notas relacionadas con enlaces de Obsidian.
- Añade cada tema nuevo al índice `00 - Inicio.md`.
- Evita incluir credenciales, identificadores de cuenta u otros datos sensibles.

## Aviso

Este repositorio es material de estudio independiente. No está afiliado con Amazon Web Services y no sustituye la documentación oficial ni la guía vigente del examen.
