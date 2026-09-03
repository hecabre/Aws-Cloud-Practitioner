# Amazon Route 53

**Amazon Route 53** es un servicio DNS altamente disponible y escalable. Traduce nombres de dominio a destinos, como direcciones IP o recursos de AWS, y puede dirigir el tráfico según distintas políticas.

Route 53 permite registrar dominios, alojar registros en zonas hospedadas públicas o privadas y realizar comprobaciones de estado. Una zona hospedada privada responde a nombres de dominio dentro de las VPC asociadas.

## Políticas de enrutamiento

- Enrutamiento basado en latencia.
- Enrutamiento por geolocalización.
- Enrutamiento ponderado (weighted).
- Enrutamiento por conmutación por error (failover).
- Enrutamiento basado en geoproximidad.

Las políticas determinan la respuesta DNS; no sustituyen los controles de seguridad ni garantizan por sí solas que el destino esté disponible. Las comprobaciones de estado pueden participar en decisiones de enrutamiento compatibles.
