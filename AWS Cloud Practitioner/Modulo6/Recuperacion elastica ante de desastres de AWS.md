# AWS Elastic Disaster Recovery

AWS Elastic Disaster Recovery (AWS DRS) reduce el tiempo de inactividad y la pérdida de datos al facilitar la recuperación en AWS de aplicaciones ejecutadas en servidores físicos, virtuales o basados en la nube.

## ¿Cómo funciona?

- Replica continuamente los datos de los servidores de origen a un área de preparación de bajo costo en AWS.
- Permite realizar simulacros de recuperación sin interrumpir el entorno de origen.
- Ante un desastre, coordina el lanzamiento de instancias de recuperación en AWS desde un punto de recuperación seleccionado.
- Después de resolver el incidente, permite realizar la conmutación por recuperación hacia la infraestructura de origen.
