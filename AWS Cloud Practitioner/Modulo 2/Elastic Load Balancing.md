# Elastic Load Balancing

Elastic Load Balancing (ELB) distribuye automáticamente el tráfico entrante entre varios destinos saludables, como instancias de [[Amazon EC2]], contenedores o direcciones IP, en una o varias zonas de disponibilidad.

El balanceador funciona como un único punto de contacto para los clientes. Supervisa el estado de los destinos registrados mediante comprobaciones de estado y dirige el tráfico a los que considera saludables.

## Alcance

- Puede configurarse como público, para recibir tráfico desde Internet, o como interno.
- Escala automáticamente la capacidad del propio balanceador conforme cambia el tráfico.
- No agrega ni elimina instancias EC2: esa función corresponde a [[Amazon EC2 Auto Scaling]].

## Relación con Amazon EC2 Auto Scaling

Ambos servicios se complementan:

1. Amazon EC2 Auto Scaling ajusta la cantidad de instancias de acuerdo con la demanda.
2. Las instancias se registran o eliminan del grupo de destinos del balanceador.
3. Elastic Load Balancing distribuye las solicitudes entre los destinos saludables.

Usar destinos en varias [[Regiones y Zonas de Disponibilidad|zonas de disponibilidad]] ayuda a mantener la disponibilidad si una zona o un destino falla.

## Enrutamiento

El algoritmo depende del tipo de balanceador:

- Un **Application Load Balancer** usa round robin de forma predeterminada y también admite least outstanding requests y weighted random.
- Un **Network Load Balancer** selecciona el destino mediante un hash basado en el flujo de la conexión.

## Ventajas

- Es un servicio administrado: AWS se encarga de la infraestructura y el escalado del balanceador.
- Utiliza comprobaciones de estado para dirigir el tráfico a destinos saludables.
- Facilita distribuir la carga entre múltiples destinos y zonas de disponibilidad.
