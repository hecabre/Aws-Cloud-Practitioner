# Instantáneas de Amazon EBS

Las **instantáneas de Amazon EBS** son copias de seguridad en un momento determinado de los volúmenes de [[Amazon Elastic Block Store (EBS)]]. Se almacenan administrativamente en Amazon S3, en buckets a los que el usuario no accede directamente mediante la consola ni la API de S3.

## ¿Cómo funcionan?

- La primera instantánea de un volumen incluye todos los bloques escritos.
- Las instantáneas posteriores son incrementales: guardan sólo los bloques nuevos o modificados desde la instantánea anterior.
- Aunque el almacenamiento es incremental, cada instantánea puede utilizarse para restaurar el estado completo del volumen en ese punto.
- Una instantánea permite crear volúmenes en otras zonas de disponibilidad. También puede copiarse a otra región para crear allí nuevos volúmenes.

> [!important]
> AWS no crea automáticamente copias de seguridad de todos los volúmenes EBS. La automatización debe configurarse mediante [[Amazon Data Lifecycle Manager]] o AWS Backup.
