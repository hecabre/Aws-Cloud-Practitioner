# AWS Storage Gateway

AWS Storage Gateway es un servicio de **almacenamiento híbrido** que conecta aplicaciones locales con servicios de almacenamiento de AWS mediante protocolos estándar.

## ¿Cómo funciona?

Utiliza un dispositivo de gateway virtual o físico y mantiene una caché local para ofrecer acceso de baja latencia a los datos más utilizados.

Ofrece tres tipos principales de soluciones:

- **Gateway de archivos:** proporciona acceso mediante NFS o SMB y almacena los datos en servicios como [[Amazon S3]].
- **Gateway de volúmenes:** presenta volúmenes mediante iSCSI y permite almacenar copias de los datos en AWS.
- **Gateway de cintas:** reemplaza bibliotecas de cintas físicas por cintas virtuales almacenadas en AWS.
