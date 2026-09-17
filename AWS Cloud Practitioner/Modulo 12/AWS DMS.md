# AWS Database Migration Service (AWS DMS)

## ¿Qué es?

AWS DMS es un servicio administrado para descubrir, evaluar, convertir y migrar datos entre bases de datos, almacenes de datos y otros almacenes compatibles. Permite realizar migraciones únicas o replicar cambios continuos para mantener sincronizados el origen y el destino.

> [!note]
> En una migración heterogénea, además de mover los datos puede ser necesario convertir el esquema y los objetos de código mediante DMS Schema Conversion o [[AWS SCT]].

## Beneficios

- Reduce el tiempo de inactividad mediante la replicación continua.
- Admite migraciones homogéneas, entre motores iguales, y heterogéneas, entre motores diferentes compatibles.
- Administra la infraestructura de replicación y ofrece un modelo de pago por uso.

## Casos de uso

- Migrar o modernizar bases de datos.
- Replicar cambios continuos entre almacenes de datos.
- Integrar datos con almacenes analíticos y lagos de datos compatibles.
