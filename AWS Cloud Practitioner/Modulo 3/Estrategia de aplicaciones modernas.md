# Estrategia de aplicaciones modernas

La elección entre un modelo operativo **sin servidor** y **Kubernetes** busca equilibrar la autonomía de los equipos, la estandarización y los recursos dedicados a operar las cargas de trabajo.

AWS recomienda evaluar la opción de cómputo **para cada carga de trabajo**, dentro de la estrategia operativa de la organización. No es obligatorio utilizar un solo enfoque: distintos equipos o aplicaciones pueden usar modelos diferentes.

## Consideraciones principales

### 1. Estructura y habilidades de la organización

- **Equipos distribuidos:** cada equipo desarrolla, despliega y opera sus aplicaciones. Favorecen la autonomía y la innovación a su propio ritmo.
- **Equipo centralizado:** mantiene estándares, crea automatizaciones y comparte prácticas recomendadas.
- **Equipo de plataforma:** crea y mantiene una plataforma interna con herramientas comunes de despliegue, automatización y observabilidad. Este modelo suele relacionarse con Kubernetes y Amazon EKS.

Se debe considerar la experiencia disponible en desarrollo, automatización, operaciones, DevOps, SRE y Kubernetes. En equipos con pocos recursos operativos, el modelo sin servidor puede reducir la administración de infraestructura.

### 2. Modelo operativo y herramientas

La organización debe decidir qué herramientas estandarizar para crear, configurar, desplegar, proteger y observar sus cargas de trabajo.

- El modelo sin servidor puede utilizar herramientas como AWS SAM, AWS CDK o AWS CloudFormation.
- Kubernetes utiliza su API y puede apoyarse en herramientas de GitOps, como Argo CD, además de herramientas de su ecosistema.

Mantener demasiadas herramientas aumenta la carga operativa. Conviene estandarizar un conjunto que cubra la mayoría de los patrones de trabajo.

### 3. Características de la carga de trabajo

Cada carga debe evaluarse según sus requisitos de:

- Rendimiento.
- Seguridad.
- Resiliencia.
- Costos.
- Escalamiento.
- Entorno de ejecución y capacidad de cómputo.

La estrategia debe admitir casos como microservicios, monolitos modernizados, arquitecturas basadas en eventos, procesamiento por lotes, streaming y aprendizaje automático. Algunas cargas de IA o ML pueden necesitar instancias especializadas o GPU.

### 4. Integraciones

Se debe revisar la integración con bases de datos, mensajería, streaming, orquestación y otros servicios.

- [[Aws Lambda]] ofrece integraciones administradas y encaja especialmente bien con arquitecturas basadas en eventos.
- Amazon EKS permite trabajar con servicios de AWS y con el amplio ecosistema de herramientas de código abierto de Kubernetes.

La mejor alternativa depende de si la organización prioriza las integraciones administradas de AWS o la compatibilidad con el ecosistema y las API de Kubernetes.

### 5. Prototipado

La estrategia debe permitir crear, desplegar y validar ideas rápidamente.

- AWS Lambda y AWS App Runner reducen las decisiones iniciales y la carga operativa, por lo que facilitan el prototipado rápido.
- Kubernetes también puede utilizarse para prototipos, pero normalmente requiere que un equipo de plataforma prepare clústeres o espacios de nombres y simplifique la experiencia de despliegue.

## ¿Cuándo considerar cada enfoque?

| Sin servidor | Kubernetes |
| --- | --- |
| Se prefieren los servicios y herramientas administrados de AWS | Kubernetes es la interfaz principal de la plataforma de cómputo |
| Se busca transferir a AWS la mayor cantidad posible de operación de infraestructura | Existe un equipo de plataforma central con habilidades especializadas |
| Los desarrolladores necesitan autonomía y concentrarse en escribir código | Se necesita estandarizar cargas mediante las API y herramientas de Kubernetes |
| Se quieren acelerar prototipos y reducir la carga operativa | Se valora el ecosistema de la CNCF y sus proyectos de código abierto |
| Ejemplos: Amazon ECS, AWS App Runner, AWS Fargate y [[Aws Lambda]] | Ejemplos: Amazon EKS y Red Hat OpenShift Service on AWS |

> [!important] Idea clave
> La elección depende principalmente del modelo operativo y de las capacidades del equipo, no solo de las características técnicas del servicio. Muchas cargas pueden ejecutarse correctamente con cualquiera de los dos enfoques.

## Preguntas para tomar la decisión

1. ¿Los equipos operan sus propias aplicaciones o existe un equipo central de plataforma?
2. ¿La organización ya posee experiencia y herramientas de Kubernetes?
3. ¿Cuánto trabajo de infraestructura se desea transferir a AWS?
4. ¿Qué rendimiento, seguridad, resiliencia y costo exige la carga?
5. ¿Qué integraciones de AWS o del ecosistema de código abierto necesita?
6. ¿Qué tan rápido debe poder prototiparse y desplegarse?

## Relacionado

- [[Aws Lambda]]
- [[Servicio administrado]]
- [[Servicio completamente administrado]]
- [[Arquitectura de Microservicios]]
- [[Arquitectura Debilmente Acoplada]]
