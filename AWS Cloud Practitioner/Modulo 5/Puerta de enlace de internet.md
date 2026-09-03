# Puerta de enlace de Internet

Una **puerta de enlace de Internet** es un componente de Amazon VPC que permite la comunicación entre la VPC e Internet.

Para que una subred sea pública, su tabla de enrutamiento debe incluir una ruta hacia la puerta de enlace de Internet. Además, los recursos necesitan una dirección IP pública o IPv6 y reglas de seguridad que permitan el tráfico correspondiente. La puerta de enlace, por sí sola, no hace públicos todos los recursos de la VPC.

La puerta de enlace de Internet se adjunta a la VPC y proporciona el destino de Internet para las rutas IPv4 (`0.0.0.0/0`) o IPv6 (`::/0`). También realiza la traducción entre direcciones IPv4 públicas y privadas cuando corresponde.
