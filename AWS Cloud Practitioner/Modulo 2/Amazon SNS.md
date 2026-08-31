# Amazon SNS

Amazon Simple Notification Service (Amazon SNS) es un servicio administrado de mensajería **publicación/suscripción (pub/sub)**. Los publicadores envían mensajes a un **tema** y SNS los entrega de forma asíncrona a sus suscriptores.

Un mismo mensaje puede distribuirse a varios suscriptores, lo que se conoce como **fanout**.

## Suscriptores

Un tema puede entregar mensajes a distintos tipos de puntos de conexión, entre ellos:

- Colas de [[Amazon SQS]].
- Funciones Lambda.
- Puntos de conexión HTTP o HTTPS.
- Correo electrónico.
- SMS y notificaciones push móviles.

## Diferencia con Amazon SQS

- **Amazon SNS:** envía cada mensaje a los suscriptores del tema mediante un modelo push.
- **[[Amazon SQS]]:** conserva los mensajes en una cola hasta que un consumidor los recibe y elimina, o hasta que vence su periodo de retención.

SNS aplica políticas de reintento cuando una entrega falla. Para conservar mensajes que no pudieron entregarse, se puede asociar una cola de mensajes fallidos de Amazon SQS a la suscripción.
