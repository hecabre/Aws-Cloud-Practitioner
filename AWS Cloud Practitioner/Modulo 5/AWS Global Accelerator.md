# AWS Global Accelerator

**AWS Global Accelerator** utiliza la red global de AWS para mejorar la disponibilidad y el rendimiento de las aplicaciones para usuarios de todo el mundo.

Enruta el tráfico hacia los puntos de conexión adecuados y puede realizar una conmutación por error rápida cuando detecta problemas en los puntos de conexión de la aplicación.

Proporciona direcciones IP estáticas anycast que anuncian puntos de presencia de AWS. El acelerador recibe el tráfico en la ubicación de borde más cercana y lo lleva por la red global de AWS hasta un endpoint regional, como un balanceador de carga, una instancia EC2 o una dirección IP elástica. No es una CDN: no almacena contenido en caché.
