# Almacenamiento de objetos

El **almacenamiento de objetos** guarda los datos como unidades independientes dentro de un espacio de nombres plano. Está diseñado para almacenar grandes cantidades de datos no estructurados sin tener que administrar la capacidad física.

## Estructura de un objeto

Cada objeto incluye:

- los datos;
- una clave o identificador único;
- metadatos que facilitan su organización, búsqueda y recuperación.

Los objetos se agrupan en contenedores llamados **buckets**. Para actualizar los datos, normalmente se reemplaza el objeto en lugar de modificar bloques individuales.

## Casos de uso

Es apropiado para archivos grandes o que no cambian con frecuencia, copias de seguridad, contenido multimedia y conjuntos de datos no estructurados.

## Servicio relacionado

- [[Amazon S3]]
