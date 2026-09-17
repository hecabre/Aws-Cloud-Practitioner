# Ataques de DDoS

## ¿Qué son?

Un ataque distribuido de denegación de servicio (**DDoS**) utiliza múltiples sistemas para enviar tráfico o solicitudes excesivas a un objetivo e impedir el acceso de usuarios legítimos.

## Mitigación en AWS

- **AWS Shield:** detecta y mitiga ataques DDoS en recursos compatibles.
- **[[Elastic Load Balancing]]:** distribuye el tráfico entre varios destinos saludables.
- **[[AWS Cloud Practitioner/Modulo 5/Amazon Cloudfront|Amazon CloudFront]] y [[Amazon Route 53]]:** aprovechan la infraestructura global de AWS para absorber y distribuir tráfico.
- **AWS WAF:** filtra solicitudes web según reglas configurables.

> [!note]
> Los grupos de seguridad filtran tráfico a nivel de instancia, pero no sustituyen a un servicio especializado de protección contra DDoS.
