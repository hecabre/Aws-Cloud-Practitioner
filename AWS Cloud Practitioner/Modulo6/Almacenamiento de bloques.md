# Almacenamiento de bloques

El **almacenamiento de bloques** divide los datos en fragmentos de tamaño fijo llamados bloques, cada uno con una dirección única. El sistema operativo puede tratar un volumen de bloques como si fuera un disco físico.

## Características

- Permite leer o modificar bloques individuales sin reemplazar todo el archivo.
- Ofrece baja latencia y es adecuado para sistemas operativos, aplicaciones y bases de datos que requieren actualizaciones frecuentes.

## Opciones para Amazon EC2

- **Almacén de instancias de [[Amazon EC2]]:** almacenamiento temporal conectado físicamente al host. Los datos persisten durante un reinicio, pero no si la instancia se detiene, hiberna o termina. No debe utilizarse como almacenamiento duradero.
- **[[Amazon Elastic Block Store (EBS)]]:** proporciona volúmenes persistentes fuera de la instancia que se conectan a instancias EC2.

Amazon EBS permite crear snapshots como copias de seguridad y cifrar los volúmenes. Con Elastic Volumes, también se puede aumentar el tamaño, cambiar el tipo o ajustar el rendimiento de un volumen compatible sin desconectarlo ni reiniciar la instancia.
