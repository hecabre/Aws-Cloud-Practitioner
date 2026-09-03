# ACL de red

Una **ACL de red** es un firewall virtual que permite o deniega tráfico entrante y saliente a nivel de subred.

Las ACL de red no tienen estado: las reglas de entrada y salida se evalúan por separado, por lo que el tráfico de respuesta debe permitirse explícitamente.

Una ACL se asocia a una subred y sus reglas se evalúan en orden numérico ascendente hasta encontrar una coincidencia. Puede contener reglas de permiso y denegación. La ACL predeterminada permite todo el tráfico, mientras que una ACL personalizada comienza con reglas que deniegan el tráfico hasta que se agreguen permisos.
