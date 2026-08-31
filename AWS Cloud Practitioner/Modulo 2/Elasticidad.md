# Elasticidad

La elasticidad es la capacidad de aumentar o reducir los recursos para ajustarlos a la demanda actual o prevista.

En una arquitectura elástica, los recursos pueden aprovisionarse cuando aumenta la carga y liberarse cuando disminuye. Esto evita mantener permanentemente la capacidad necesaria para el pico máximo.

Por ejemplo, un grupo de [[Amazon EC2 Auto Scaling]] puede aplicar [[Escalado Horizontal|escalado horizontal]]:

- **Scale out:** agrega instancias cuando aumenta la demanda.
- **Scale in:** elimina instancias cuando disminuye la demanda.

La elasticidad ayuda a conservar el rendimiento y a utilizar los recursos de manera eficiente, pero el ahorro depende de que los recursos que ya no se necesitan se reduzcan o eliminen correctamente.

## Diferencia con escalabilidad

La [[Escalabilidad]] indica si un sistema puede aumentar su capacidad. La elasticidad añade la capacidad de ajustar esa capacidad dinámicamente conforme cambia la demanda.
