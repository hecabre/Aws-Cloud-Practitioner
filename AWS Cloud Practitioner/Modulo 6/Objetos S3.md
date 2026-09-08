# Objetos de Amazon S3

## ¿Qué es un objeto?

Un objeto es la unidad fundamental de almacenamiento de [[Amazon S3]]. Cada objeto contiene:

- los datos;
- metadatos del sistema y definidos por el usuario;
- una clave que lo identifica de forma única dentro de un bucket;
- un identificador de versión, cuando S3 Versioning está habilitado;
- información de control de acceso.

Aunque la clave puede parecer el nombre de un archivo o incluir prefijos similares a carpetas, S3 utiliza un espacio de nombres plano.
