# Amazon Elastic Container Service (ECS)

Amazon Elastic Container Service (Amazon ECS) es un [[Servicio completamente administrado]] de orquestación de contenedores que permite desplegar, administrar y escalar aplicaciones en contenedores.

ECS administra el plano de control y el programador de tareas. El cliente define las imágenes, los recursos, la red y el comportamiento de las aplicaciones.

## Opciones de capacidad

- **[[AWS Fargate]]:** ejecuta contenedores sin administrar servidores ni planificar la capacidad de instancias.
- **[[Amazon EC2]]:** permite elegir los tipos de instancia y controlar la capacidad, pero el cliente administra las instancias.
- **ECS Managed Instances:** permite utilizar tipos de instancia de EC2 mientras AWS administra su aprovisionamiento, escalamiento, aplicación de parches y ciclo de vida.

## ¿Cuándo es ideal?

Es una opción adecuada cuando se busca una orquestación de contenedores integrada con AWS sin administrar un plano de control. La opción de capacidad se elige según el nivel de control y de administración de infraestructura requerido.

## Escalamiento

ECS puede escalar tareas y capacidad mediante funciones de escalamiento que deben configurarse según las métricas y necesidades de la aplicación; no aumenta ni disminuye todos los recursos automáticamente por el solo hecho de utilizar el servicio.

## Relacionado

- [[Contenedores]]
- [[Amazon Elastic Container Registry (ECR)]]
- [[AWS Fargate]]
- [[Amazon Elastic Kubernetes Service (EKS)]]
