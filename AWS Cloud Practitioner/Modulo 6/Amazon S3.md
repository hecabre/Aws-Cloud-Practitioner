# Amazon Simple Storage Service (Amazon S3)

Amazon Simple Storage Service (Amazon S3) es un [[Servicio completamente administrado|servicio completamente administrado]] y escalable de [[Almacenamiento de objetos|almacenamiento de objetos]] al que se accede mediante API y protocolos web.

El tamaño máximo de un objeto es de 5 TB. En una única operación `PUT` se pueden cargar hasta 5 GB; para objetos mayores se utiliza la carga multiparte.

Amazon S3 está diseñado para ofrecer un 99,999999999 % de durabilidad de los objetos. También ofrece características para optimizar costos y proteger datos, como control de versiones, administración del ciclo de vida y distintas clases de almacenamiento.

## Características

1. Los buckets y objetos son privados de forma predeterminada; el acceso debe concederse explícitamente mediante políticas u otros mecanismos.
2. Las URL prefirmadas conceden acceso temporal a una operación sin modificar la política de bucket.
3. Los puntos de acceso simplifican la administración del acceso compartido a conjuntos de datos.
4. Las solicitudes pueden auditarse mediante registros de acceso al servidor o eventos de datos de AWS CloudTrail.
## Conceptos principales

- Los datos se almacenan como **objetos**.
- Cada objeto contiene los datos, una clave única dentro del bucket y metadatos.
- Los objetos se organizan dentro de **buckets** creados en una región de AWS.
- Un bucket y sus objetos son privados de forma predeterminada; el acceso se concede explícitamente mediante políticas y otros mecanismos.
- S3 Versioning puede conservar varias versiones de un objeto y ayudar a recuperarlo después de una eliminación o sobrescritura accidental.

Amazon S3 se utiliza, entre otros casos, para copias de seguridad, archivos, contenido web, lagos de datos y análisis.
