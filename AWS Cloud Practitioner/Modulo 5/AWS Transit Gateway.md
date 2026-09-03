# AWS Transit Gateway

**AWS Transit Gateway** actúa como un concentrador central para conectar varias VPC y redes locales, en lugar de enlazarlas entre sí individualmente.

Las conexiones se realizan mediante attachments, por ejemplo de VPC, VPN, Direct Connect o peering. Transit Gateway usa tablas de enrutamiento propias para controlar qué attachments pueden comunicarse; una VPC conectada no queda automáticamente autorizada para comunicarse con todas las demás.

A medida que la infraestructura crece, se pueden interconectar Transit Gateways de distintas Regiones mediante la infraestructura global de AWS.
