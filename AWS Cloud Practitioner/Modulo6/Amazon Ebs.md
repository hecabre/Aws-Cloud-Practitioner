# Amazon EBS: casos de uso y beneficios

Esta nota amplía los conceptos principales de [[Amazon Elastic Block Store (EBS)]]. Los volúmenes EBS funcionan como discos virtuales de almacenamiento en bloques para [[Amazon EC2]] y persisten independientemente del ciclo de ejecución de una instancia.

Al crear un volumen, se eligen su tamaño, tipo y configuración de rendimiento. El volumen y la instancia a la que se conecta deben encontrarse en la misma zona de disponibilidad. Su rendimiento puede expresarse mediante métricas como **IOPS** y **rendimiento de transferencia** (*throughput*).

> [!important]
> Los volúmenes EBS no se almacenan en buckets de [[Amazon S3]]. Las **instantáneas de EBS** sí se almacenan administrativamente en Amazon S3, pero no son accesibles desde la consola ni la API de S3.

## Casos de uso

- Almacenamiento para bases de datos.
- Volúmenes raíz y datos de aplicaciones.
- Entornos de desarrollo que requieren almacenamiento persistente y flexible.

## Beneficios

1. **Migración de datos:** una instantánea permite crear un volumen en otra zona de disponibilidad. También se puede copiar a otra región y crear allí un volumen.
2. **Cambio de instancia:** un volumen puede desconectarse y volver a conectarse a otra instancia compatible de la misma zona de disponibilidad, sin perder sus datos.
3. **Recuperación ante desastres:** las instantáneas periódicas permiten restaurar volúmenes desde puntos anteriores. La frecuencia y el tiempo de restauración deben ajustarse a los objetivos de recuperación de la carga.
4. **Optimización de costos:** Elastic Volumes permite ajustar el tipo y aumentar el tamaño del volumen de acuerdo con el uso real, dentro de las operaciones compatibles.
5. **Ajuste del rendimiento:** los distintos tipos de volumen permiten elegir características de IOPS y throughput acordes con la carga de trabajo.

## Relacionado

- [[Instantaneas de Amazon EBS|Instantáneas de Amazon EBS]]
- [[Amazon Data Lifecycle Manager]]
