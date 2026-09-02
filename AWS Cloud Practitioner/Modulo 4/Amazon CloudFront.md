# Amazon CloudFront

**Amazon CloudFront** es una red de entrega de contenido (CDN) que distribuye contenido estático y dinámico, como imágenes, videos, sitios web y respuestas de API, desde ubicaciones cercanas a los usuarios para reducir la latencia.

## Cómo funciona

1. El usuario solicita contenido de una aplicación o sitio web.
2. La solicitud se dirige al punto de presencia de CloudFront que puede atenderla con menor latencia.
3. Si el contenido está en caché, CloudFront lo entrega directamente.
4. Si no está en caché, CloudFront lo solicita al **origen**, lo entrega al usuario y puede almacenarlo para solicitudes posteriores.

El origen puede ser, por ejemplo, un bucket de Amazon S3, un balanceador de carga, una instancia de Amazon EC2 u otro servidor HTTP.

## Ubicaciones de borde

Las **ubicaciones de borde**, también llamadas puntos de presencia o **PoP**, son instalaciones de la red global de AWS desde las que CloudFront entrega contenido a los usuarios. Las cachés regionales de borde complementan estos puntos y reducen la necesidad de volver al origen.

> [!note]
> El contenido no tiene que estar siempre almacenado en caché: CloudFront también puede acelerar la entrega de contenido dinámico mediante la red global de AWS.
