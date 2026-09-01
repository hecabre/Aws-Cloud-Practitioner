# Servicio no administrado

Un **recurso administrado principalmente por el cliente**, llamado de forma simplificada “no administrado”, es aquel en el que el cliente conserva más responsabilidades operativas.

El término no significa que AWS deje de administrar la infraestructura de la nube. Describe la parte del recurso que el cliente debe operar.

El cliente puede tener que encargarse de:

- Configurar y mantener el sistema operativo.
- Instalar aplicaciones y dependencias.
- Aplicar parches y actualizaciones dentro del recurso.
- Configurar el escalamiento, la disponibilidad y el monitoreo.

## Ejemplo: Amazon EC2

En [[Amazon EC2]], AWS administra la infraestructura física, la red y el hipervisor. El cliente administra el sistema operativo invitado, las aplicaciones, los parches del sistema operativo y gran parte de la configuración de seguridad.

Por eso, una instancia de EC2 se considera **administrada principalmente por el cliente** y requiere más trabajo operativo que [[Aws Lambda]]. AWS sigue administrando la infraestructura física y la capa de virtualización que la hacen funcionar.

## Idea clave

> “No administrado” no significa que AWS no tenga ninguna responsabilidad; significa que el cliente conserva una mayor parte de la administración operativa.

## Comparación rápida

| Nivel | Quién realiza la operación | Ejemplo |
| --- | --- | --- |
| Administrado principalmente por el cliente | AWS opera la infraestructura física; el cliente administra el sistema operativo y la aplicación | [[Amazon EC2]] |
| [[Servicio administrado]] | AWS asume una cantidad de tareas que depende del servicio; el cliente conserva las demás | Amazon RDS |
| Servicio abstracto o [[Servicio completamente administrado|completamente administrado]] | AWS opera la infraestructura, el sistema operativo y la plataforma; el cliente configura y usa el servicio | [[Aws Lambda]] |

## Relacionado

- [[Servicio administrado]]
- [[Servicio completamente administrado]]
- [[Responsabilidad Compartida]]
- [[Amazon EC2]]
