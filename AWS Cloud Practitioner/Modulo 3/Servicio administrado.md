# Servicio administrado

Un **servicio administrado** es aquel en el que AWS se encarga de una parte importante de las tareas operativas de la infraestructura subyacente.

Según el servicio, AWS puede encargarse de:

- Aprovisionar y mantener servidores.
- Aplicar parches al sistema o a la plataforma.
- Proporcionar alta disponibilidad y escalamiento.
- Reemplazar la infraestructura que presenta fallos.

Esto permite que el cliente se concentre más en su aplicación y sus datos. Sin embargo, el cliente todavía debe configurar el servicio correctamente, controlar los accesos y proteger la información, de acuerdo con el [[Responsabilidad Compartida|modelo de responsabilidad compartida]].

## Grados de administración

**Administrado** es un concepto amplio: AWS asume tareas operativas cuya cantidad depende del servicio. No representa siempre un nivel intermedio formal. Los servicios pueden entenderse como un espectro de responsabilidad:

| Grado | Responsabilidad del cliente | Ejemplo |
| --- | --- | --- |
| Administrado principalmente por el cliente | Administra el sistema operativo invitado, las aplicaciones y sus datos | [[Amazon EC2]] |
| Servicio administrado | AWS automatiza tareas operativas específicas y el cliente conserva las responsabilidades indicadas para el servicio | Amazon RDS |
| Servicio abstracto o [[Servicio completamente administrado|completamente administrado]] | AWS opera la infraestructura, el sistema operativo y la plataforma; el cliente configura y utiliza el servicio | [[Aws Lambda]], Amazon S3 y Amazon DynamoDB |

## Idea clave

> Cuanto más administrado es un servicio, más responsabilidades operativas se transfieren a AWS.

> [!important] Responsabilidad compartida
> Incluso en un servicio completamente administrado, el cliente sigue siendo responsable de aspectos como sus datos, identidades, permisos y configuración.

## Relacionado

- [[Servicio no administrado]]
- [[Servicio completamente administrado]]
- [[Aws Lambda]]
- [[Amazon EC2]]
