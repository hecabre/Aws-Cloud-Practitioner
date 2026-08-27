# Responsabilidad Compartida

La seguridad en AWS es una responsabilidad **compartida entre AWS y el cliente**.

## AWS es responsable de la seguridad de la nube

- Instalaciones físicas.
- Hardware e infraestructura global.
- Sistema operativo del host.
- Capa de virtualización.
- Redes y controles de los servicios gestionados.

## El cliente es responsable de la seguridad en la nube

- Sistema operativo invitado.
- Aplicaciones y su configuración.
- Datos del cliente.
- Gestión de identidades y accesos, como IAM.
- Reglas de firewall y grupos de seguridad.

> El reparto exacto cambia según el servicio: en **IaaS** el cliente administra más; en **PaaS** menos; en **SaaS** AWS se encarga de casi todo y el cliente protege principalmente sus datos y accesos.

## Relacionado

- [[Computación en la Nube]]
- [[Amazon EC2]]
- [[00 - Inicio]]
