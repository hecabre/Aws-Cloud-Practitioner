# AWS Lambda

AWS Lambda es un servicio de cómputo **sin servidor** y [[Servicio completamente administrado|completamente administrado]] que ejecuta código en respuesta a eventos o solicitudes, sin necesidad de aprovisionar ni administrar servidores.

Lambda administra automáticamente la infraestructura subyacente, los entornos de ejecución, el escalamiento, el enrutamiento y la tolerancia a fallos. Esto permite concentrarse en la lógica de la aplicación.

## ¿Cuándo es ideal?

Es adecuado para aplicaciones basadas en eventos, API, procesamiento de datos y tareas de automatización que puedan ejecutarse dentro de sus límites de duración.

## Duración

El tiempo de espera de una función se configura entre 1 segundo y un máximo de **900 segundos (15 minutos)** por invocación.

Si un proceso requiere más tiempo, puede dividirse en varias tareas o utilizarse otra opción de cómputo que se adapte mejor a la carga de trabajo.

## Precio

Lambda utiliza un modelo de pago por uso. En las funciones, el costo considera las solicitudes y la duración de la ejecución, medida según la memoria asignada y el tiempo consumido.

## Ventajas

- Escala automáticamente en respuesta a la demanda.
- Se integra con numerosos servicios de AWS mediante eventos.
- Permite utilizar tiempos de ejecución proporcionados por Lambda o crear uno personalizado.
- La memoria configurada también determina la cantidad de CPU disponible, por lo que ajustarla puede influir en el rendimiento.

## ¿Cómo funciona?

1. Se crea una función de Lambda.
2. Se carga el código y se configura su entorno de ejecución.
3. Se conecta una fuente de eventos o un disparador.
4. Lambda ejecuta la función cuando recibe el evento o la solicitud.

Los disparadores pueden provenir de servicios como [[Amazon SQS]], [[Amazon SNS]] o [[Amazon Event Bridge]].

## Responsabilidad operativa

En comparación con [[Amazon EC2]], Lambda transfiere más tareas operativas a AWS. El cliente todavía debe administrar el código, la configuración, los permisos y los datos de la aplicación, de acuerdo con el [[Responsabilidad Compartida|modelo de responsabilidad compartida]].

## Relacionado

- [[Estrategia de aplicaciones modernas]]
- [[Servicio administrado]]
- [[Servicio completamente administrado]]
- [[Servicio no administrado]]
