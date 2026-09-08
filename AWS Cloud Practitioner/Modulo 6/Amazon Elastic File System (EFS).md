# Amazon Elastic File System (EFS)

Amazon Elastic File System (Amazon EFS) es un [[Servicio completamente administrado|servicio completamente administrado]], sin servidor y elástico de [[Almacenamiento de archivos|almacenamiento de archivos]] compartido.

Utiliza NFSv4 y permite que varios recursos de cómputo de AWS accedan al mismo sistema de archivos. Sus clientes son principalmente sistemas Linux; no admite el montaje desde instancias EC2 basadas en Windows.

También puede montarse desde servidores locales conectados a una VPC mediante AWS Direct Connect o AWS Site-to-Site VPN.

## Diferencias respecto de Amazon EBS

- Varias instancias pueden leer y escribir simultáneamente en el mismo sistema de archivos.
- Utiliza NFS y está orientado principalmente a clientes Linux.
- Puede ser un recurso Regional o One Zone.
- Su capacidad de almacenamiento crece y se reduce automáticamente.

## Características

- Crece y se reduce automáticamente al agregar o eliminar archivos, sin aprovisionar capacidad por adelantado.
- Un sistema de archivos **Regional** almacena datos de forma redundante en varias zonas de disponibilidad; **One Zone** los almacena en una sola zona.
- Admite varios clientes concurrentes, por lo que resulta apropiado para directorios compartidos, sistemas de contenido y aplicaciones web.

## Clases de almacenamiento

EFS combina dos tipos de sistema de archivos con clases de almacenamiento según la frecuencia de acceso:

- **Regional:** almacena los datos de forma redundante en varias zonas de disponibilidad. Admite las clases EFS Standard, EFS Infrequent Access (IA) y EFS Archive.
- **One Zone:** almacena los datos en una sola zona de disponibilidad a menor costo. Admite EFS One Zone y EFS One Zone-IA, pero no EFS Archive.

EFS Lifecycle Management puede mover automáticamente archivos de Standard a IA o Archive según su patrón de acceso.
