# AWS CloudTrail

## ¿Qué es?

Es un servicio que registra la actividad de una cuenta de AWS. Captura acciones realizadas mediante la consola, la CLI, los SDK y las API, lo que permite saber quién hizo qué, cuándo y desde dónde.

## Beneficios

- Facilita la auditoría y el cumplimiento.
- Ayuda a supervisar la seguridad e investigar incidentes.
- Permite solucionar problemas operativos y rastrear cambios.

## Historial de eventos

CloudTrail está habilitado de forma predeterminada para consultar el **historial de eventos**. Este historial ofrece un registro consultable, descargable e inmutable de los últimos 90 días de eventos de administración en cada región, sin cargos por consultarlo.

> [!important]
> El historial de eventos no sustituye a un trail: para conservar eventos durante más tiempo, incluir otros tipos de eventos o centralizar registros, se debe crear un trail o un almacén de datos de eventos.

## Trails

Un **trail** entrega los eventos seleccionados a un bucket de [[Amazon S3]] y, de forma opcional, a otros destinos compatibles. Esto permite conservar y analizar los registros durante el periodo requerido.

## CloudTrail Insights

CloudTrail Insights analiza patrones habituales de actividad de escritura de la API y genera eventos cuando detecta actividad inusual, como cambios en el volumen de llamadas o en las tasas de error.
