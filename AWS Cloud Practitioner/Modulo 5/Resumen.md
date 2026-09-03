# Resumen de redes de AWS

| Servicio | Descripción |
| --- | --- |
| [[Amazon VPC]] | Sección lógicamente aislada de la nube de AWS donde se pueden lanzar recursos en una red virtual definida por el usuario. |
| [[Subredes]] | Sección de una [[Amazon VPC]] que contiene recursos y ayuda a organizarlos como públicos o privados. |
| [[Puerta de enlace de internet]] | Componente que permite la comunicación entre una VPC e Internet cuando la ruta, las direcciones y las reglas de seguridad están configuradas. |
| [[Puertas de enlace privadas virtuales]] | Componente del lado de AWS que permite una conexión Site-to-Site VPN entre una VPC y una red privada aprobada. |
| [[Amazon Client VPN]] | Servicio de red elástico y [[Servicio completamente administrado]] para conectar de forma segura a trabajadores remotos con los recursos de AWS. |
| [[AWS Site-To-Site VPN]] | Crea una conexión segura mediante túneles VPN entre las instalaciones físicas y los recursos de AWS. |
| [[Aws Private Link]] | Tecnología escalable y de alta disponibilidad para conectar de forma privada una VPC con servicios y recursos. |
| [[AWS Direct Connect]] | Proporciona una conexión de red dedicada entre una red local y AWS. |
| [[ACL]] | Permite o deniega tráfico entrante o saliente a nivel de subred; no tiene estado. |
| [[Grupos de seguridad]] | Controlan el tráfico entrante y saliente a nivel de instancia; tienen estado. |
| [[DNS]] | Traduce nombres de dominio a destinos, como direcciones IP. |
| [[Amazon Route 53]] | Servicio DNS escalable y fiable para registrar dominios, dirigir tráfico y comprobar el estado de los recursos. |
| [[AWS Global Accelerator]] | Mejora la disponibilidad y el rendimiento mediante el enrutamiento del tráfico a través de la red global de AWS. |
| [[Puerta de enlace NAT]] | Permite que las instancias de una subred privada se conecten con servicios externos; esos servicios no pueden iniciar conexiones con las instancias. |
| [[Amazon API Gateway]] | Servicio para crear, publicar, mantener, supervisar y proteger API a cualquier escala. |
| [[AWS Transit Gateway]] | Actúa como un concentrador central para conectar varias VPC y redes locales. |
| [[Amazon Cloudfront]] | Red de entrega de contenido (CDN) que distribuye contenido mediante ubicaciones de borde para reducir la latencia. |
| [[Diagramas de AWS]] | Explica los elementos habituales de los diagramas de AWS, como Regiones, VPC y subredes. |
| [[Ejemplos]] | Presenta un ejemplo de entrega de contenido a varias Regiones a nivel global. |
| [[Fortalecimiento de la red]] | Describe el uso de ACL de red y grupos de seguridad para controlar el tráfico. |
| [[Tabla de enrutamiento]] | Contiene reglas que determinan hacia dónde se dirige el tráfico de una subred o una puerta de enlace. |
