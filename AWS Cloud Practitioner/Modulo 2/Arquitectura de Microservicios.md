# Arquitectura de microservicios

En una arquitectura de microservicios, una aplicación se divide en servicios pequeños e independientes, orientados a capacidades específicas del negocio.

Los servicios se comunican mediante interfaces bien definidas, como API o eventos, y pueden desarrollarse, desplegarse y escalarse de forma independiente.

## Ventajas

- Permite escalar sólo los servicios que necesitan más capacidad.
- Reduce el alcance de los cambios y facilita despliegues independientes.
- Favorece una [[Arquitectura Debilmente Acoplada]] y el aislamiento de fallos.

El fallo de un microservicio no tiene que detener toda la aplicación, pero esto no ocurre automáticamente: depende de que existan límites de fallo, reintentos y mecanismos de comunicación resilientes.

## Consideración

Los microservicios añaden complejidad operativa porque forman un sistema distribuido y requieren administrar la comunicación, observabilidad y coordinación entre servicios.

## Relacionado

- [[Aplicaciones Monoliticas]]
- [[Amazon Event Bridge]]
- [[Amazon SQS]]
