# Contenedores

Un contenedor es una unidad de software ligera y portable que empaqueta una aplicación junto con las dependencias que necesita para ejecutarse correctamente.

## Diferencia frente a las máquinas virtuales

A diferencia de una máquina virtual tradicional, un contenedor no necesita incluir un sistema operativo completo. Los contenedores comparten el kernel del sistema operativo del equipo anfitrión, pero mantienen aislados sus procesos y dependencias.

## Almacenamiento y ejecución

[[Amazon Elastic Container Registry (ECR)]] almacena las imágenes de los contenedores. Los servicios como [[Amazon Elastic Container Service (ECS)]] y [[Amazon Elastic Kubernetes Service (EKS)]] orquestan su ejecución.

Los contenedores pueden ejecutarse sobre distintas opciones de cómputo:

- **[[Amazon EC2]]:** ofrece mayor control sobre las instancias, pero el cliente administra más infraestructura.
- **[[AWS Fargate]]:** ejecuta contenedores sin que el cliente aprovisione ni administre servidores.

## Relacionado

- [[Amazon Elastic Container Registry (ECR)]]
- [[Amazon Elastic Container Service (ECS)]]
- [[Amazon Elastic Kubernetes Service (EKS)]]
- [[AWS Fargate]]
