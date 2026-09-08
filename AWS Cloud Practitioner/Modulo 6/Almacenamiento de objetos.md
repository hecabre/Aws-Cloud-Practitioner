# Almacenamiento de objetos

El **almacenamiento de objetos** guarda los datos como unidades independientes dentro de un espacio de nombres plano. Está diseñado para escalar a grandes cantidades de datos no estructurados sin tener que administrar la infraestructura de almacenamiento física.

## Estructura de un objeto

Cada objeto incluye:

- los datos;
- una clave o identificador único;
- metadatos que describen el objeto y facilitan su administración.

Los objetos se agrupan en contenedores llamados **buckets**. A diferencia del almacenamiento de bloques, una actualización normalmente reemplaza el objeto completo en lugar de modificar bloques individuales.

## Casos de uso

Es apropiado para copias de seguridad, contenido multimedia, contenido web, lagos de datos y otros conjuntos de datos no estructurados.

## Servicio relacionado

- [[Amazon S3]]
