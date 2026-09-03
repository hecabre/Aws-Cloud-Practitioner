# Diagramas de AWS

![[Pasted image 20260903083834.png]]

## Elementos del diagrama

1. **Nube de AWS:** es el cuadro más grande en la mayoría de los diagramas.
2. **Región y Zonas de disponibilidad:** son las ubicaciones que elegimos según nuestros requisitos.
3. **Amazon VPC:** es la red aislada y segmentada lógicamente dentro de AWS; suele representarse con un cuadro de líneas sólidas.
4. **Subredes:** son fragmentos de la VPC que permiten dividirla en secciones más pequeñas y fáciles de administrar. Una subred es, básicamente, un rango de direcciones IP dentro de la VPC y pertenece a una única Zona de disponibilidad.

## Subredes privadas

Se utilizan para aislar recursos que no deberían exponerse directamente a Internet pública. En los diagramas se representan como cuadros con líneas sólidas.

## Subredes públicas

Se utilizan para recursos que necesitan acceso a Internet mediante una ruta hacia una puerta de enlace de Internet; además, los recursos necesitan una dirección IP pública o IPv6 y reglas de seguridad adecuadas. Una ruta por sí sola no expone un recurso a Internet. En los diagramas se representan como cuadros de líneas discontinuas.
