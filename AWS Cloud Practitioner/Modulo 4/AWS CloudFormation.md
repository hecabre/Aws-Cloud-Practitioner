# AWS CloudFormation e infraestructura como código

La **infraestructura como código (IaC)** permite definir y administrar infraestructura mediante archivos de configuración. Así se puede repetir una configuración de forma uniforme, reducir variaciones manuales y conservar sus cambios junto con el código.

## ¿Qué es AWS CloudFormation?

**AWS CloudFormation** es un servicio de IaC que permite modelar recursos de AWS de forma declarativa mediante plantillas en YAML o JSON.

En la plantilla se describe el estado deseado de los recursos y sus propiedades. CloudFormation interpreta esa definición y llama a las API correspondientes para aprovisionarlos y configurarlos.

## Conceptos principales

- **Plantilla:** archivo que describe los recursos y la configuración deseada.
- **Stack:** conjunto de recursos que CloudFormation administra como una sola unidad.
- **Implementación repetible:** una misma plantilla puede reutilizarse para crear entornos con una configuración coherente.

> [!important]
> CloudFormation administra los recursos definidos en la plantilla, pero una actualización puede modificar, interrumpir o reemplazar recursos según las propiedades que cambien.
