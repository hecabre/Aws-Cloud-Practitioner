# Ejemplos de arquitectura de red

## Entrega de contenido a varias regiones a nivel global

### Servicios utilizados

1. Usamos [[Amazon Route 53]] para dirigir el tráfico a [[AWS Cloud Practitioner/Modulo 5/Amazon Cloudfront|Amazon CloudFront]].
2. [[AWS Cloud Practitioner/Modulo 5/Amazon Cloudfront|Amazon CloudFront]] distribuye el contenido mediante una ubicación de borde cercana al usuario.
3. Si el contenido no está en caché, CloudFront lo solicita al origen configurado, que puede estar en una [[Regiones y Zonas de Disponibilidad|Región]] de AWS.
4. La [[Amazon VPC]] y sus controles de red regulan el acceso a los recursos de origen, como las instancias [[Amazon EC2]].

![[Pasted image 20260903160743.png]]

