# Amazon DynamoDB

## ¿Qué es?

Amazon DynamoDB es una [[Base de datos NoSQL|base de datos NoSQL]] sin servidor y [[Servicio completamente administrado|completamente administrada]]. Ofrece tiempos de respuesta de milisegundos de un solo dígito a cualquier escala.

Las **tablas globales de DynamoDB** proporcionan replicación multi-Región y multi-activa. Es ideal para aplicaciones que requieren alto rendimiento y escalado con poca sobrecarga operativa, y se utiliza en eventos de gran escala como Amazon Prime Day.
## Casos de uso
1. Plataformas de juegos.
2. Aplicaciones de servicios financieros.
3. Aplicaciones móviles con bases de usuarios globales.
## Beneficios
1. El modo bajo demanda ajusta automáticamente la capacidad, mientras que el modo aprovisionado permite usar auto scaling con un objetivo de utilización.
2. Ofrece tiempos de respuesta de milisegundos de un solo dígito a cualquier escala.
3. De forma predeterminada, replica los datos entre tres zonas de disponibilidad de una región y ofrece un SLA de disponibilidad del 99.99 %. Las tablas globales configuradas en varias regiones pueden ofrecer un SLA del 99.999 %.
4. Cifra todos los datos en reposo de forma predeterminada y permite elegir entre claves propiedad de AWS, administradas por AWS o administradas por el cliente. El tráfico de red utiliza HTTPS para proteger los datos en tránsito.
