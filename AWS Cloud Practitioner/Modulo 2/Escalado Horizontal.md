# Escalado horizontal

El escalado horizontal consiste en agregar más instancias o nodos para repartir una carga de trabajo. La reducción de esos recursos se conoce como **scale in**.

Este enfoque permite procesar más trabajo en paralelo y evita depender de una sola máquina. En AWS, [[Amazon EC2 Auto Scaling]] puede agregar o eliminar instancias y [[Elastic Load Balancing]] puede distribuir el tráfico entre ellas.

La aplicación debe estar diseñada para distribuir el trabajo y administrar correctamente el estado compartido entre los recursos.

## Relacionado

- [[Escalabilidad]]
- [[Elasticidad]]
- [[Escalado Vertical]]
