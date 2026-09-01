# Servicio completamente administrado

Un **servicio completamente administrado** es aquel en el que AWS se encarga de operar la infraestructura y la plataforma necesarias para prestar el servicio. El cliente consume la funcionalidad sin administrar servidores, sistemas operativos ni el mantenimiento de la plataforma.

AWS se encarga normalmente de:

- Aprovisionar y mantener la infraestructura.
- Aplicar parches a la plataforma subyacente.
- Reemplazar los recursos que presentan fallos.
- Proporcionar disponibilidad y escalamiento propios del servicio.

El cliente todavía es responsable de:

- Configurar correctamente el servicio.
- Administrar identidades y permisos.
- Proteger y clasificar sus datos.
- Escribir código o definir reglas cuando el servicio lo requiera.
- Controlar el uso y los costos.

## Ejemplos

- [[Aws Lambda]]: el cliente proporciona el código y AWS administra los servidores y el entorno de ejecución.
- [[Amazon SQS]]: el cliente crea y configura las colas; AWS opera la infraestructura del sistema de mensajería.
- [[Amazon SNS]]: el cliente configura temas y suscripciones; AWS opera la infraestructura de publicación y entrega.
- [[Elastic Load Balancing]]: el cliente configura el balanceador; AWS administra su infraestructura y capacidad.

## Diferencia importante

**Servicio administrado** es el concepto general: AWS asume algunas tareas operativas. **Completamente administrado** indica que AWS opera todas las capas de infraestructura y plataforma del servicio, aunque el cliente conserva sus responsabilidades de configuración, acceso, código y datos.

> Completamente administrado no significa que el cliente deje de tener responsabilidades.

## Relacionado

- [[Servicio administrado]]
- [[Servicio no administrado]]
- [[Responsabilidad Compartida]]
