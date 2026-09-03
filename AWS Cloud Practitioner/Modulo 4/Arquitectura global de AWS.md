# Arquitectura global de AWS

La infraestructura global de AWS se organiza en **Regiones**, **Zonas de disponibilidad (AZ)** y una red global de **puntos de presencia**. Esta distribución permite diseñar cargas de trabajo con baja latencia, elasticidad y alta disponibilidad.

## Beneficios principales

- **Alta disponibilidad:** capacidad de una carga de trabajo para continuar cumpliendo su función pese a ciertas fallas, con el menor tiempo de inactividad posible.
- **Agilidad:** capacidad de adaptar e implementar infraestructura con rapidez cuando cambian los requisitos.
- **Elasticidad:** capacidad de agregar o retirar recursos según la demanda. Puede aplicarse mediante escalado horizontal o vertical; consulta [[Elasticidad]] y [[Escalabilidad]].

## Regiones

Una **Región de AWS** es un área geográfica separada que contiene varias Zonas de disponibilidad físicamente independientes y conectadas mediante redes de baja latencia y alta capacidad.

Las Regiones están aisladas entre sí. Los recursos y datos creados en una Región no se replican automáticamente en otra, salvo que se configure una función de replicación o copia del servicio correspondiente.

### Cómo elegir una Región

1. **Requisitos legales y de conformidad:** algunas cargas de trabajo deben mantener sus datos en una ubicación determinada.
2. **Proximidad y latencia:** una Región cercana a la mayoría de los usuarios puede reducir el tiempo de respuesta.
3. **Disponibilidad de servicios y características:** no todos están disponibles en todas las Regiones.
4. **Precio:** el costo de un mismo servicio puede variar entre Regiones.

## Redundancia y alta disponibilidad

La **redundancia** evita puntos únicos de falla al disponer de componentes alternativos.

- Una arquitectura **Multi-AZ** distribuye recursos entre varias Zonas de disponibilidad de una misma Región. Si una AZ presenta una interrupción, la carga puede continuar en otra, siempre que los recursos, la replicación y la conmutación por error estén configurados correctamente.
- Una arquitectura **multi-Región** puede proteger frente a una interrupción regional, pero requiere replicar los datos y configurar el enrutamiento o la conmutación por error entre Regiones.

> [!note]
> Alta disponibilidad no significa que una aplicación nunca falle; busca reducir la frecuencia y la duración de las interrupciones.

## Red global de borde

Los puntos de presencia acercan ciertos servicios de AWS a los usuarios. Entre ellos se encuentran [[AWS Cloud Practitioner/Modulo 4/Amazon CloudFront]], Amazon Route 53 y AWS Global Accelerator.

AWS Outposts cumple un propósito diferente: extiende infraestructura y servicios de AWS a las instalaciones locales del cliente; no es una ubicación de borde de la red global.
