# Tabla de enrutamiento

Una **tabla de enrutamiento** contiene reglas que determinan hacia dónde se dirige el tráfico de una subred o una puerta de enlace.

Cada ruta especifica un destino, normalmente un rango CIDR, y un objetivo, como una puerta de enlace de Internet, una puerta de enlace NAT, una conexión VPN u otra VPC.

Cada tabla contiene una ruta local para permitir la comunicación dentro de los rangos CIDR de la VPC. Cada subred se asocia con una sola tabla a la vez; si no se especifica otra, usa la tabla principal. AWS aplica la ruta más específica cuando varias rutas coinciden.
