# Amazon SQS

Amazon Simple Queue Service (Amazon SQS) es un servicio administrado de colas de mensajes que permite integrar y desacoplar componentes de software.

## Flujo básico

1. Un productor envía un mensaje a la cola.
2. SQS almacena el mensaje de forma redundante hasta que un consumidor lo elimina o vence su periodo de retención.
3. Un consumidor recibe el mensaje mediante sondeo y lo procesa.
4. El consumidor elimina el mensaje de la cola después de procesarlo correctamente.

Mientras un consumidor procesa un mensaje, el **tiempo de espera de visibilidad** evita temporalmente que otros consumidores lo reciban.

## Tipos de colas

- **Estándar:** ofrece entrega al menos una vez y orden de mejor esfuerzo, por lo que una aplicación debe tolerar mensajes duplicados o fuera de orden.
- **FIFO:** conserva estrictamente el orden dentro de cada grupo de mensajes y evita que SQS introduzca duplicados.

Amazon SQS facilita una [[Arquitectura Debilmente Acoplada]] porque el productor y el consumidor no tienen que ejecutarse al mismo tiempo ni comunicarse directamente.

## Relacionado

- [[Amazon SNS]]
- [[Amazon Event Bridge]]
