# AWS PrivateLink

## Problema

En ocasiones, otras empresas o VPC necesitan conectarse de forma privada a servicios y recursos sin exponerlos a Internet.

## Qué es

**AWS PrivateLink** es una tecnología escalable y de alta disponibilidad que conecta una VPC con servicios y recursos mediante direcciones IP privadas, como si estuvieran en la propia VPC. No requiere una puerta de enlace de Internet, un dispositivo NAT, una conexión de Direct Connect ni una VPN Site-to-Site para esa comunicación.

El consumidor controla los puntos de conexión, servicios y recursos específicos a los que se puede acceder desde la VPC.

El consumidor normalmente crea un punto de conexión de interfaz, que genera interfaces de red con direcciones IP privadas en las subredes seleccionadas. AWS PrivateLink también incluye puntos de conexión de Gateway Load Balancer y de recurso; los puntos de conexión de gateway para Amazon S3 y DynamoDB no usan PrivateLink.

## Beneficios y caso de uso

Ayuda a proteger el tráfico y simplifica la administración. Se utiliza para conectar clientes de una VPC con servicios de AWS, servicios de otras VPC o servicios ofrecidos por otras cuentas.
