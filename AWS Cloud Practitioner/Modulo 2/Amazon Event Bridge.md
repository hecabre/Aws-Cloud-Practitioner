# Amazon EventBridge

Amazon EventBridge es un servicio sin servidor que utiliza buses de eventos para conectar aplicaciones mediante eventos. Facilita la creación de arquitecturas distribuidas, escalables y basadas en eventos.

## Flujo básico

1. Una aplicación personalizada, un servicio de AWS o un proveedor de software como servicio (SaaS) envía un evento a un **bus de eventos**.
2. Las **reglas** comparan el evento con patrones definidos.
3. Si existe una coincidencia, EventBridge dirige el evento a uno o varios **destinos**, como funciones Lambda, colas de [[Amazon SQS]] o temas de [[Amazon SNS]].

Este enrutamiento permite que productores y consumidores permanezcan desacoplados: el productor no necesita conocer la implementación de los destinos.
