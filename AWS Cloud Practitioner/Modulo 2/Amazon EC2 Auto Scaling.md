# Amazon EC2 Auto Scaling

Amazon EC2 Auto Scaling ayuda a mantener la cantidad adecuada de instancias de [[Amazon EC2]] disponibles para gestionar la carga de una aplicación.

Las instancias se organizan en un **grupo de Auto Scaling**, que puede lanzar o terminar instancias según la demanda. También supervisa su estado y reemplaza las instancias no saludables para mantener la capacidad deseada.

## Capacidades del grupo

1. **Capacidad mínima:** límite inferior configurado para el grupo. La capacidad deseada no se reduce por debajo de este valor.
2. **Capacidad deseada:** cantidad de instancias que el grupo intenta mantener. Debe encontrarse entre la capacidad mínima y la máxima.
3. **Capacidad máxima:** límite superior configurado para el grupo. De forma predeterminada, la capacidad deseada no aumenta por encima de este valor.

## Métodos de escalado

- **Manual:** se modifica directamente la capacidad deseada.
- **Programado:** cambia la capacidad en fechas u horarios conocidos.
- **Dinámico:** responde a cambios actuales en la demanda mediante políticas y métricas.
- **Predictivo:** analiza patrones históricos y aprovisiona capacidad antes de la demanda prevista.

El escalado dinámico es reactivo y el predictivo es proactivo; se pueden utilizar juntos.

## Relación con Elastic Load Balancing

[[Amazon EC2 Auto Scaling]] ajusta la cantidad de instancias, mientras que [[Elastic Load Balancing]] distribuye el tráfico entre los destinos saludables. Si el grupo abarca varias [[Regiones y Zonas de Disponibilidad|zonas de disponibilidad]], puede distribuir las instancias entre ellas y contribuir a la alta disponibilidad.

## Relacionado

- [[Escalado Horizontal]]
- [[Elasticidad]]
- [[Escalabilidad]]
