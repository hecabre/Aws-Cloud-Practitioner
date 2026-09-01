# Amazon Elastic Kubernetes Service (EKS)

Amazon Elastic Kubernetes Service (Amazon EKS) es un servicio administrado para ejecutar Kubernetes en AWS y en entornos híbridos.

En el modo estándar, AWS administra el **plano de control de Kubernetes**. La administración de los nodos donde se ejecutan los pods depende de la opción de cómputo elegida.

## Opciones de cómputo

- **EKS estándar con [[Amazon EC2]]:** ofrece mayor control sobre los nodos, sus tipos de instancia y su configuración. El cliente conserva más responsabilidades operativas.
- **EKS con [[AWS Fargate]]:** ejecuta pods sin que el cliente aprovisione ni administre servidores.
- **EKS Auto Mode:** amplía la administración de AWS al plano de datos y automatiza el aprovisionamiento, escalamiento y mantenimiento de los nodos, además de componentes de red y almacenamiento.

## ¿Cuándo es ideal?

Es adecuado cuando Kubernetes es la interfaz principal de la plataforma, se necesita su ecosistema y existe experiencia para configurar y operar las cargas de trabajo de Kubernetes.

## Idea clave

> Que EKS sea un servicio administrado no significa que AWS administre todos los componentes en todas sus modalidades. El reparto de responsabilidades cambia entre EKS estándar, Fargate y EKS Auto Mode.

## Relacionado

- [[Estrategia de aplicaciones modernas]]
- [[Contenedores]]
- [[Amazon Elastic Container Registry (ECR)]]
- [[Amazon Elastic Container Service (ECS)]]
