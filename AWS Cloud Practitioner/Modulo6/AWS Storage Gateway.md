# AWS Storage Gateway

AWS Storage Gateway es un servicio de **almacenamiento híbrido** que conecta aplicaciones locales con servicios de almacenamiento de AWS mediante protocolos estándar.

## ¿Cómo funciona?

Se implementa como un dispositivo virtual, un dispositivo físico o una instancia de Amazon EC2. Según el tipo de gateway, utiliza almacenamiento local como caché o búfer para facilitar el acceso a los datos y su transferencia a AWS.

Ofrece tres tipos principales de soluciones:

- **Gateway de archivos:** S3 File Gateway proporciona acceso mediante NFS o SMB y almacena los archivos como objetos en [[Amazon S3]]. FSx File Gateway proporciona acceso SMB a Amazon FSx for Windows File Server, aunque ya no está disponible para clientes nuevos.
- **Gateway de volúmenes:** presenta almacenamiento en bloques mediante iSCSI y crea snapshots de los volúmenes en AWS.
- **Gateway de cintas:** presenta una biblioteca de cintas virtuales mediante iSCSI y permite archivar las cintas virtuales en AWS.
