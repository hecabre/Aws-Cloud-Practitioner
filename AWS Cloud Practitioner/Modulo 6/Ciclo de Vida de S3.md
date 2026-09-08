# Ciclo de vida de Amazon S3

## ¿Qué es?

Las configuraciones de S3 Lifecycle permiten automatizar la administración de uno o varios [[Objetos S3]] mediante reglas. Existen dos tipos principales de acciones:

1. **Acciones de transición:** definen cuándo los objetos pasan a otra clase de almacenamiento.
2. **Acciones de vencimiento:** definen cuándo los objetos vencen y Amazon S3 debe eliminarlos.

En un bucket con control de versiones, las reglas pueden tratar de forma diferente las versiones actuales y las no actuales; por ello, el vencimiento no siempre equivale a la eliminación permanente inmediata de todos los datos del objeto.
