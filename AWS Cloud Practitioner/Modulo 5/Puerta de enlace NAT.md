# Puerta de enlace NAT

Una **puerta de enlace de traducción de direcciones de red (NAT)** permite que las instancias de una subred privada se conecten con servicios externos.

Una puerta de enlace NAT pública se crea en una subred pública y necesita una dirección IPv4 elástica. La tabla de enrutamiento de la subred privada debe dirigir el tráfico hacia ella; la NAT, a su vez, usa una ruta hacia la puerta de enlace de Internet. Los servicios externos no pueden iniciar conexiones con esas instancias.

Una puerta de enlace NAT se crea en una Zona de disponibilidad. Para evitar que una interrupción afecte a otras Zonas, se recomienda usar una NAT por Zona y enrutar cada subred hacia la NAT de su propia Zona. Para IPv6 se utilizan normalmente una puerta de enlace de Internet de salida (egress-only) o NAT64 según el caso.
