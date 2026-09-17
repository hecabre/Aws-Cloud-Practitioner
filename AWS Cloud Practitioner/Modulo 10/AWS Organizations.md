# AWS Organizations

## ¿Qué es?

Es un servicio que permite administrar varias cuentas de AWS de forma centralizada. Las cuentas pueden agruparse en unidades organizativas para aplicar políticas, compartir recursos y consolidar la facturación.

## Beneficios

- Automatiza la creación y administración de cuentas.
- Facilita la aplicación centralizada de controles.
- Consolida la facturación y ayuda a analizar los costos de las cuentas.

## Casos de uso

- Crear y organizar cuentas de AWS a escala.
- Proporcionar acceso y herramientas a los equipos de seguridad.
- Compartir recursos entre cuentas.
- Establecer límites de permisos mediante políticas de control de servicios.

## Políticas de control de servicios (SCP)

Una **SCP** establece los permisos máximos disponibles para usuarios y roles de IAM en las cuentas miembro afectadas. Puede limitar servicios, recursos y acciones de API, pero **no concede permisos por sí misma**: los permisos deben concederse mediante políticas de IAM o políticas basadas en recursos.
