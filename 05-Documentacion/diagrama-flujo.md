# Diagrama de Flujo – Botón de Pánico

```mermaid
flowchart TD
    A[Usuario presiona botón de pánico] --> B[Aplicación envía señal al servidor]
    B --> C{¿Servidor recibe señal?}
    C -- Sí --> D[Servidor procesa alerta]
    D --> E[Se registra en la base de datos]
    E --> F[Se envía notificación a contactos/entidad de seguridad]
    F --> G[Confirmación de recepción]
    G --> H[Fin del proceso]
    C -- No --> I[Reintento de envío]
    I --> B


