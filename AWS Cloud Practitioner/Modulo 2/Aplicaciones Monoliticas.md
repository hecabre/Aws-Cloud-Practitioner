# Aplicaciones monolíticas

Una aplicación monolítica se construye y despliega como una sola unidad. Sus componentes suelen ejecutarse juntos y compartir dependencias, por ejemplo:

- Base de datos.
- Interfaz.
- Lógica de negocio.

Debido a que sus componentes suelen estar [[Arquitectura Estrechamente Acoplada|estrechamente acoplados]], un cambio o fallo puede tener un impacto amplio en la aplicación. Además, normalmente se escala la aplicación completa aunque sólo uno de sus componentes necesite más capacidad.

Una arquitectura monolítica puede ser válida para ciertos casos; su principal diferencia frente a una [[Arquitectura de Microservicios]] es que no divide la aplicación en servicios que puedan desplegarse y escalarse de forma independiente.
