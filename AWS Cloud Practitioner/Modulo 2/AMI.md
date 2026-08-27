# Amazon Machine Image (AMI)

## ¿Qué es?

Una **AMI** es una imagen que proporciona el software necesario para configurar y arrancar una instancia de [[Amazon EC2]]. Para lanzar una instancia se debe especificar una AMI compatible con el tipo de instancia elegido.

Una AMI define, entre otros elementos:

- El sistema operativo y el software instalado.
- La arquitectura del procesador.
- El mapeo de dispositivos de bloques, que indica los volúmenes que se adjuntarán al iniciar la instancia.
- Los permisos de lanzamiento, que controlan qué cuentas pueden usarla.

> [!important]
> Una AMI es específica de una región, aunque puede copiarse a otra.

## Ventajas

Las AMI permiten lanzar varias instancias con una configuración coherente y repetible.

## ¿Cómo se obtienen?

Las AMI se pueden obtener de varias maneras:

- Crear una AMI propia a partir de una instancia EC2.
- Usar una AMI proporcionada por AWS, pública o compartida por otra cuenta.
- Comprar una AMI en AWS Marketplace.

## Relacionado

- [[Amazon EC2]]
- [[Tipos de Instancias]]
- [[00 - Inicio]]
