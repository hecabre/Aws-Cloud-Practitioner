# Amazon Elastic Block Store (EBS)

Amazon Elastic Block Store (Amazon EBS) proporciona volúmenes persistentes de [[Almacenamiento de bloques|almacenamiento de bloques]] que se conectan a instancias de [[Amazon EC2]] como si fueran discos físicos.

## ¿Para qué sirve?

- **Volumen raíz:** puede almacenar el sistema operativo y los programas de una instancia EC2.
- **Volumen de datos:** permite guardar archivos y datos de aplicaciones.
- **Copias de seguridad:** permite crear snapshots de un volumen en un momento determinado.

## Características

- Un volumen EBS conserva sus datos cuando la instancia se detiene o reinicia.
- Cuando una instancia termina, la conservación del volumen depende de la configuración **DeleteOnTermination**. El volumen raíz se elimina de forma predeterminada, aunque este comportamiento se puede cambiar.
- Cada volumen se crea en una zona de disponibilidad específica y se replica automáticamente dentro de esa zona para protegerlo ante el fallo de un componente.
- El volumen sólo puede conectarse a instancias de la misma zona de disponibilidad. Normalmente se conecta a una instancia a la vez; determinados volúmenes Provisioned IOPS SSD admiten **Multi-Attach** a varias instancias de la misma zona.
- Con Elastic Volumes y una instancia compatible, se puede aumentar el tamaño, cambiar el tipo o ajustar el rendimiento sin desconectar el volumen ni reiniciar la instancia.

> [!important]
> La replicación automática dentro de una zona de disponibilidad no reemplaza las copias de seguridad mediante snapshots.

## Relacionado

- [[Amazon Ebs|Casos de uso y beneficios de Amazon EBS]]
- [[Instantaneas de Amazon EBS|Instantáneas de Amazon EBS]]
- [[Amazon Data Lifecycle Manager]]
