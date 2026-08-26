# Regiones y Zonas de Disponibilidad

## Región

- Es una **ubicación física** en el mundo donde se agrupan centros de datos.
- Sirve para acercar los recursos a los usuarios y cumplir requisitos de residencia de datos.
- Cada región opera de forma independiente.

## Zona de disponibilidad

- Es uno o varios centros de datos **aislados y físicamente separados** dentro de una región.
- Están conectados entre sí mediante redes de baja latencia.
- Una región de AWS tiene, como mínimo, **tres zonas de disponibilidad**.

## ¿Por qué usar varias zonas de disponibilidad?

- Permiten lograr **alta disponibilidad**.
- Si una zona falla, la aplicación puede seguir funcionando en otra.
- Son la base de arquitecturas tolerantes a fallos y de la replicación de datos.

> Las **ubicaciones de borde** complementan la infraestructura global: acercan contenido a los usuarios con servicios como **Amazon CloudFront** y reducen la latencia.

## Relacionado

- [[Amazon EC2]]
- [[00 - Inicio]]
