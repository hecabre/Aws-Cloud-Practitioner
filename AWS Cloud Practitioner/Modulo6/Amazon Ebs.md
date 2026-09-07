## Que es?
Es un servicio de AWS que puede crear discos duros virtuales llamados volumenes EBS, que podemos adjuntar al volumen de datos de [[Amazon EC2]]. Estan separados de los volumenes del volumen de la instancia [[Amazon EC2]] y no estan vinculados fisicamente al host de [[Amazon EC2]], pueden persistir entre paradas e inicios de EC2.
Defines el tamano, tipo y configuracion. Despues se adjunta al [[Amazon EC2]]
El rendimiento se mide en IOPS, entrada y salidas 
## Casos de uso
Algunos casos de usos de amazon EBS son:
1. Alojamiento de bases de datos
2. Almacenamiento de copias de seguridad para aplicaciones
3. Implementacion agil de entornos de desarrollo

## Beneficios
Los volumenes EBS admiten la portabilidad de datos gracias a la capacidad para desconectarse y volver a conectarse a las instancias segun sea necesario. Hay michas razones practicas por las que puede optar por hacer esto.
1. Migracion de datos: Se pueden migrar los datos entre zonas de disponibilidad mediante instantaneas. Las instaneas permiten mover datos entre regiones o crear copias de forma sencilla
2. Cambios en los tipos de instancias: Como permiten aislados de las instancias [[Amazon EC2]], no es complicado conectarlos a distintos tipos de instancias. Esta flexibilidad le permite aumentar o reducir la categoria de las instnacias sin perder datos
3. Recuperacion de desastres: Las instantaneas de EBS proporcionan soluciones de copias de segfuridad confiables que se pueden restaurar en diferentes regiones durante las emergencias. Las instaneas automatizadas regulares garantizan que sus datos permanezcan protegidos y se pueden recuperar de inmediato
4. Optimizacion de costos: Se pueden modificar en cuanto a tipo y tamano para que se ajusten a los patrones de usos reales. Pueden alternar entre tipos de almacenamiento ajustar la capacidad sin tiempo de actividad
5. Ajuste de rendimiento: Amazon EBS ofrece muchso tipos de volumenes para adaptarse a los diferentes requisitos de carga de trabajo y necesidades de IOPS. Puede ajustar las caracteristias de rendimiento del volumen sobre la marcha para satisfaces las demandas cambiandes de las aplicaciones