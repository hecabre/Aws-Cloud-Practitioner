# Subredes

Una **subred** es un rango de direcciones IP dentro de una [[Amazon VPC]]. Se utiliza para organizar recursos y puede ser pública o privada según su tabla de enrutamiento.

Cada subred se crea en una única Zona de disponibilidad. Para mejorar la disponibilidad, se pueden distribuir subredes equivalentes en varias Zonas de disponibilidad. AWS reserva cinco direcciones IPv4 de cada bloque CIDR de la subred para su funcionamiento.

Por lo general, una subred privada contiene recursos que no deben exponerse directamente a Internet, como una base de datos. Una subred pública puede contener recursos orientados al cliente, como un sitio web, si tiene una ruta a una puerta de enlace de Internet y los recursos cuentan con direcciones y reglas de seguridad adecuadas. La diferencia entre pública y privada depende principalmente del enrutamiento; una subred no se vuelve pública sólo por contener una dirección IP pública.
