# Arquitectura débilmente acoplada

En una arquitectura débilmente acoplada, los componentes tienen pocas dependencias entre sí y se comunican mediante interfaces bien definidas.

Este diseño permite modificar, reemplazar o escalar un componente con un impacto mínimo en los demás. También ayuda a aislar los fallos, aunque no garantiza por sí solo que nunca se propaguen.

Cuando no se necesita una respuesta inmediata, la comunicación asíncrona mediante colas o eventos reduce todavía más la dependencia directa entre componentes. Algunos servicios que facilitan este patrón son:

- [[Amazon SQS]], mediante colas de mensajes.
- [[Amazon SNS]], mediante publicación y suscripción.
- [[Amazon Event Bridge]], mediante el enrutamiento de eventos.

Este tipo de acoplamiento es habitual en una [[Arquitectura de Microservicios]].
