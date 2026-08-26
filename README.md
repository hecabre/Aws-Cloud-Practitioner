# AWS Cloud Practitioner

Notas de estudio en español para preparar la certificación **AWS Certified Cloud Practitioner**. El repositorio está organizado como una bóveda de [Obsidian](https://obsidian.md/) y conecta los conceptos mediante enlaces internos para facilitar el repaso.

## Contenido

Actualmente, las notas cubren:

- Fundamentos de la computación en la nube.
- Modelo cliente-servidor.
- Modelo de responsabilidad compartida.
- Regiones y zonas de disponibilidad de AWS.
- Amazon EC2, virtualización, hipervisores y tenencia múltiple.
- Familias de instancias EC2 y sus principales casos de uso.
- Un resumen rápido para el repaso final.

## Cómo usar este repositorio

### Con Obsidian

1. Clona el repositorio:

   ```bash
   git clone https://github.com/hecabre/Aws-Cloud-Practitioner.git
   ```

2. Abre Obsidian y selecciona **Abrir carpeta como bóveda**.
3. Elige la carpeta raíz del repositorio.
4. Empieza por la nota [00 - Inicio](AWS%20Cloud%20Practitioner/00%20-%20Inicio.md).

Obsidian resolverá los enlaces internos con formato `[[Nombre de la nota]]` y permitirá explorar las relaciones entre temas mediante su vista de grafo.

### Desde GitHub

También puedes leer las notas directamente en GitHub. Usa [00 - Inicio](AWS%20Cloud%20Practitioner/00%20-%20Inicio.md) como índice principal y continúa con el [Resumen Rápido](AWS%20Cloud%20Practitioner/Resumen%20Rápido.md) para repasar los puntos clave.

> GitHub muestra los enlaces internos de Obsidian como texto, pero los enlaces Markdown de este README sí permiten acceder a las notas principales.

## Estructura

```text
.
├── .agents/skills/                  # Skill local para generar simulacros
├── .obsidian/                       # Configuración de la bóveda
├── AWS Cloud Practitioner/
│   ├── 00 - Inicio.md               # Índice principal
│   ├── Computación en la Nube.md
│   ├── Modelo Cliente-Servidor.md
│   ├── Responsabilidad Compartida.md
│   ├── Regiones y Zonas de Disponibilidad.md
│   ├── Amazon EC2.md
│   ├── Hipervisor.md
│   ├── Tenencia Múltiple.md
│   ├── Tipos de Instancias.md
│   ├── Tipos de Instancias/          # Detalle de cada familia EC2
│   └── Resumen Rápido.md
└── README.md
```

## Ruta de estudio sugerida

1. [Computación en la Nube](AWS%20Cloud%20Practitioner/Computaci%C3%B3n%20en%20la%20Nube.md)
2. [Modelo Cliente-Servidor](AWS%20Cloud%20Practitioner/Modelo%20Cliente-Servidor.md)
3. [Responsabilidad Compartida](AWS%20Cloud%20Practitioner/Responsabilidad%20Compartida.md)
4. [Regiones y Zonas de Disponibilidad](AWS%20Cloud%20Practitioner/Regiones%20y%20Zonas%20de%20Disponibilidad.md)
5. [Amazon EC2](AWS%20Cloud%20Practitioner/Amazon%20EC2.md)
6. [Tipos de Instancias](AWS%20Cloud%20Practitioner/Tipos%20de%20Instancias.md)
7. [Resumen Rápido](AWS%20Cloud%20Practitioner/Resumen%20R%C3%A1pido.md)

## Generar exámenes con Codex

El repositorio incluye la skill [`aws-cloud-practitioner-exams`](.agents/skills/aws-cloud-practitioner-exams/SKILL.md). Codex la detecta automáticamente al trabajar dentro del repositorio y puedes invocarla con una petición como:

```text
Usa $aws-cloud-practitioner-exams para crear un examen de simulación basado en mis notas.
```

La skill construye el temario desde las notas disponibles, genera el examen y su clave en archivos separados, y también permite calificar respuestas. Los simulacros se guardan en `AWS Cloud Practitioner/Exámenes de simulación/`.

## Contribuciones

Las mejoras, correcciones y nuevas notas son bienvenidas. Para mantener la bóveda consistente:

- Usa Markdown para el contenido.
- Escribe nombres de archivo descriptivos.
- Conecta las notas relacionadas con enlaces de Obsidian.
- Añade cada tema nuevo al índice `00 - Inicio.md`.
- Evita incluir credenciales, identificadores de cuenta u otros datos sensibles.

## Aviso

Este repositorio es material de estudio independiente. No está afiliado con Amazon Web Services y no sustituye la documentación oficial ni la guía vigente del examen.
