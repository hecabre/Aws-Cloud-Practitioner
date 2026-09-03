# Fortalecimiento de la red

Una de las principales razones para usar [[Subredes]] es controlar el acceso y segmentar el tráfico de red.

## ACL de red

Cada paquete que entra o sale de una subred se evalúa mediante la ACL de red asociada. La ACL comprueba si el tráfico coincide con una regla permitida o denegada y solo evalúa el tráfico al cruzar el límite de entrada o salida de la subred.

Una ACL de red **no tiene estado**: permitir una dirección del tráfico no permite automáticamente el tráfico de respuesta. Las reglas de entrada y salida deben permitir explícitamente el tráfico necesario.

## Grupos de seguridad

El grupo de seguridad controla el tráfico a nivel de instancia, por ejemplo, para permitir tráfico HTTP en un puerto concreto. Los grupos de seguridad tienen estado, por lo que el tráfico de respuesta se permite automáticamente.

El grupo de seguridad predeterminado permite tráfico entrante desde otros recursos asociados al mismo grupo y permite todo el tráfico saliente. Sus reglas se pueden modificar según las necesidades.

| Control | Nivel | Estado | Reglas |
| --- | --- | --- | --- |
| ACL de red | Subred | Sin estado | Permitir y denegar |
| Grupo de seguridad | Instancia | Con estado | Solo permitir |

