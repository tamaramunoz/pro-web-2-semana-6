# Tienda de Comercio Electrónico - Programación Web II (Semana 6)
Este proyecto representa una aplicación web Fullstack dinámica que integra una experiencia de usuario interactiva en el Frontend con un robusto motor de persistencia de datos en el Backend. Evolucionando desde el procesamiento básico de formularios, el sistema implementa la gestión avanzada del ciclo de vida de **Sesiones en PHP (`$_SESSION`)**, garantizando la retención, integridad y seguridad de los estados de compra de los usuarios del lado del servidor.


## Características Implementadas
1. **Operaciones y Persistencia con Sesiones en PHP:** Inicialización obligatoria del entorno mediante `session_start()` en la línea de ejecución uno de los scripts, permitiendo al servidor retener de forma segura los productos seleccionados por el cliente a través del array global `$_SESSION['carrito_tienda']`.
2. **Conexión Híbrida Asíncrona (Fetch API):** Implementación de un puente de comunicación asíncrono en JavaScript (`fetch`) dentro de `app.js`. Al presionar "Agregar al Carrito", el cliente envía silenciosamente el ID del producto al backend de PHP, permitiendo actualizar la sesión en el servidor en tiempo real sin recargar la pantalla ni perder el estado del frontend.
3. **Manejo Seguro del Ciclo de Vida y Destrucción de Datos:** Incorporación de la función nativa `unset()` para la eliminación selectiva y segura de índices específicos de la sesión (como la operación de vaciar el carrito), protegiendo la integridad de la memoria del servidor.
4. **Mitigación de Riesgos y Seguridad Financiera:** Aislamiento absoluto de la información transaccional y de precios en la "fuente de verdad" del servidor, anulando vulnerabilidades críticas en el cliente como la manipulación local de cookies o inyecciones de scripts (XSS).


## Tecnologías utilizadas:

- PHP
- JavaScript (ES6+)
- HTML5
- CSS3


## Desarrollado por:

- Tamara Muñoz
