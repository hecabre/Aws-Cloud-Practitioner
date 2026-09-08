# Amazon Elastic File System (EFS)

Amazon Elastic File System (Amazon EFS) es un [[Servicio completamente administrado|servicio completamente administrado]], sin servidor y elástico de [[Almacenamiento de archivos|almacenamiento de archivos]] compartido.

Utiliza NFSv4 y permite que varios recursos de cómputo de AWS accedan al mismo sistema de archivos. Sus clientes son principalmente sistemas Linux; no admite el montaje desde instancias EC2 basadas en Windows.

También puede montarse desde servidores locales conectados a una VPC mediante AWS Direct Connect o AWS Site-to-Site VPN.

## Características

- Crece y se reduce automáticamente al agregar o eliminar archivos, sin aprovisionar capacidad por adelantado.
- Un sistema de archivos **Regional** almacena datos de forma redundante en varias zonas de disponibilidad; **One Zone** los almacena en una sola zona.
- Admite varios clientes concurrentes, por lo que resulta apropiado para directorios compartidos, sistemas de contenido y aplicaciones web.
