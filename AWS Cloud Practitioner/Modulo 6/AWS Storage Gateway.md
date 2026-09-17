# AWS Storage Gateway

AWS Storage Gateway es un servicio de **almacenamiento híbrido** que conecta aplicaciones locales con servicios de almacenamiento de AWS mediante protocolos estándar.

## Tipos

Sus tres tipos principales son:

1. [[S3 File Gateway]]
2. [[AWS Storage Gateway|Volume Gateway]]
3. [[AWS Storage Gateway|Tape Gateway]]

## ¿Cómo funciona?

Se implementa como un dispositivo virtual, un dispositivo físico o una instancia de Amazon EC2. Según el tipo de gateway, utiliza almacenamiento local como caché o búfer para facilitar el acceso a los datos y su transferencia a AWS.

- **Gateway de archivos:** S3 File Gateway proporciona acceso mediante NFS o SMB y almacena los archivos como objetos en [[Amazon S3]].
- **Gateway de volúmenes:** presenta almacenamiento en bloques mediante iSCSI y crea snapshots de los volúmenes en AWS.
- **Gateway de cintas:** presenta una biblioteca de cintas virtuales mediante iSCSI y permite archivar las cintas virtuales en AWS.
