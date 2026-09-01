# AWS Fargate

AWS Fargate es un motor de cómputo **sin servidor** y de pago por uso para ejecutar contenedores con [[Amazon Elastic Container Service (ECS)]] o [[Amazon Elastic Kubernetes Service (EKS)]].

Con Fargate no es necesario aprovisionar ni administrar servidores o clústeres de instancias. El cliente especifica los recursos que necesita la tarea o el pod, y AWS administra la infraestructura de cómputo subyacente.

## Responsabilidades del cliente

Aunque Fargate administra los servidores, el cliente todavía configura elementos como:

- Las imágenes y aplicaciones de los contenedores.
- La CPU y memoria solicitadas.
- Las redes, los permisos y las políticas de seguridad.
- El escalamiento de las tareas o los pods cuando corresponda.

## Relacionado

- [[Contenedores]]
- [[Amazon Elastic Container Service (ECS)]]
- [[Amazon Elastic Kubernetes Service (EKS)]]
- [[Servicio completamente administrado]]
