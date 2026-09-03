# AWS Direct Connect

## Qué es

**AWS Direct Connect** establece una conexión de red dedicada entre una red local y AWS. Mediante interfaces virtuales, puede proporcionar acceso a recursos de AWS, incluida una VPC, sin depender del proveedor de Internet en el trayecto.

La conexión se establece mediante una ubicación de Direct Connect y una interfaz virtual (VIF). Una VIF privada conecta con una VPC mediante una puerta de enlace privada virtual o un Transit Gateway; una VIF pública permite acceder a servicios públicos de AWS. Direct Connect no cifra el tráfico de forma predeterminada, por lo que se puede combinar con una VPN cuando se necesita cifrado.

## Beneficios y casos de uso

- Alto ancho de banda.
- Baja latencia y una experiencia de red más constante.
- Grandes transferencias de datos.
- Aplicaciones críticas y procesamiento en tiempo real.
- Conexión de redes locales y AWS para aplicaciones que abarcan ambos entornos.

## Cómo viajan los datos

El tráfico puede viajar desde la red local, a través de **AWS Direct Connect**, hasta los recursos de AWS configurados mediante la interfaz virtual y el enrutamiento correspondientes.
