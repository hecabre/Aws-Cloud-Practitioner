# Amazon EC2

**Amazon Elastic Compute Cloud (EC2)** ofrece máquinas virtuales en la nube. En AWS, cada máquina virtual se llama **instancia**.

Para lanzar una instancia se debe especificar una **[[AMI]]** compatible con el tipo de instancia elegido.

## Características

- **Flexible**: puedes elegir sistema operativo, software, almacenamiento y red.
- **Rápida**: las instancias se lanzan en minutos.
- **Rentable**: ofrece distintos modelos de precios para adaptar el costo al patrón de uso.
- **Redimensionable**: puedes cambiar el tamaño de la instancia según la demanda.

## Opciones de precios

- **Bajo demanda**: pagas por la capacidad de cómputo durante el tiempo que la instancia está en ejecución, sin compromiso a largo plazo ni pago por adelantado.
- **Savings Plans**: ofrecen precios reducidos a cambio de comprometer un monto de gasto por hora, medido en USD/hora, durante 1 o 3 años. Pueden ofrecer ahorros de hasta un 72% frente a los precios bajo demanda.
- **Instancias reservadas**: proporcionan un descuento de facturación para una configuración de instancia durante 1 o 3 años. Las estándar ofrecen hasta un 72% de descuento y permiten pago total anticipado, parcial anticipado o sin pago anticipado. Una instancia reservada zonal también reserva capacidad en una zona de disponibilidad.
- **Spot**: utiliza capacidad EC2 disponible con descuentos de hasta un 90% frente a los precios bajo demanda. EC2 puede interrumpir la instancia si necesita recuperar la capacidad; normalmente emite un aviso con dos minutos de anticipación.

## Opciones de tenencia

- **Dedicated Host**: servidor físico dedicado que ofrece visibilidad y control sobre la ubicación de las instancias. Resulta útil para ciertos requisitos de cumplimiento o licencias por socket, núcleo o máquina virtual.
- **Instancias dedicadas**: instancias que se ejecutan en hardware dedicado a una sola cuenta de AWS, pero sin elegir ni controlar el servidor físico específico.

## Conceptos relacionados

- [[Hipervisor]]: software de virtualización que gestiona y asigna los recursos físicos del hardware a varias máquinas virtuales.
- [[Tenencia Múltiple]]: varios clientes comparten la misma infraestructura física, pero sus datos y aplicaciones permanecen aislados lógicamente.
- [[Tipos de Instancias]]: cada familia está optimizada para un tipo de carga de trabajo.

## Escalamiento

- **Vertical**: aumentar los recursos de una misma instancia, como CPU o memoria.
- **Horizontal**: añadir o quitar instancias para repartir la carga, normalmente con Auto Scaling y balanceadores de carga.

## ¿Qué puedes hacer en una instancia?

- Elegir una AMI con **Linux o Windows** y configurar el sistema operativo.
- Instalar y elegir el software que se ejecuta dentro del sistema operativo.
- Detener una instancia respaldada por Amazon EBS cuando no la necesites para dejar de pagar su cómputo. Algunos recursos asociados, como los volúmenes EBS, pueden seguir generando cargos.

## ¿Cómo se administran las instancias?

- Mediante la Consola de administración de AWS.
- Mediante AWS Command Line Interface (AWS CLI).
- Mediante las API de AWS o un AWS SDK.

## Relacionado

- [[Computación en la Nube]]
- [[Regiones y Zonas de Disponibilidad]]
- [[00 - Inicio]]
- [[AMI]]
