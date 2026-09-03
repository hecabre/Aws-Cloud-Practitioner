# AWS Site-to-Site VPN

**AWS Site-to-Site VPN** permite crear una conexión segura mediante túneles VPN entre un centro de datos o una sucursal y los recursos de AWS.

La conexión incluye un dispositivo de puerta de enlace del cliente en la red local, un recurso customer gateway que lo representa en AWS y una puerta de enlace privada virtual o un Transit Gateway en el lado de AWS. Usa IPsec y proporciona dos túneles para favorecer la disponibilidad.

## Beneficios

- Protege la comunicación entre la red local y AWS.
- Proporciona dos túneles VPN independientes para favorecer la alta disponibilidad; ambos deben configurarse correctamente en el dispositivo del cliente.
- Permite conectar ubicaciones remotas con recursos de AWS.

## Caso de uso

Puede utilizarse durante la migración de aplicaciones y para establecer comunicación segura entre ubicaciones remotas y AWS.
