
# Comparación de servicios de almacenamiento

| Servicio | ¿Qué hace? |
| --- | --- |
| Almacén de instancias de [[Amazon EC2]] | Proporciona almacenamiento temporal conectado al host. Los datos sobreviven a un reinicio, pero se pierden al detener, hibernar o terminar la instancia. |
| [[Amazon Elastic Block Store (EBS)]] | Proporciona volúmenes persistentes de [[Almacenamiento de bloques|almacenamiento de bloques]] que se conectan a instancias de [[Amazon EC2]]. |
| [[Instantaneas de Amazon EBS|Instantáneas de Amazon EBS]] | Son copias en un momento determinado de los volúmenes EBS que permiten proteger y restaurar datos. |
| [[Amazon S3]] | Proporciona almacenamiento de objetos escalable accesible mediante API web. |
| Clases de almacenamiento de S3 | Ofrecen opciones para acceso frecuente, infrecuente y archivo, según los requisitos de acceso, recuperación y costo. |
| [[Amazon Elastic File System (EFS)]] | Proporciona un sistema de archivos elástico y completamente administrado al que pueden acceder varios recursos simultáneamente. |
| [[Amazon FSx]] | Proporciona sistemas de archivos administrados basados en Windows File Server, Lustre, NetApp ONTAP y OpenZFS. |
| [[AWS Storage Gateway]] | Integra entornos locales con servicios de almacenamiento de AWS. |
| [[S3 File Gateway]] | Proporciona acceso local mediante NFS o SMB a archivos almacenados como objetos de [[Amazon S3]], con caché local para los datos frecuentes. |
| [[Tape Gateway]] | Presenta una biblioteca de cintas virtuales compatible con aplicaciones de copias de seguridad basadas en cinta y archiva cintas en AWS. |
| [[Volume Gateway]] | Presenta volúmenes de almacenamiento en bloques mediante iSCSI y ofrece modos almacenado y en caché. |
