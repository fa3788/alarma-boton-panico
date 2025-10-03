# Análisis del Proyecto: Sistema de Alarma de Botón de Pánico

## 1. Contextualización de la necesidad
La seguridad ciudadana es una de las principales preocupaciones en entornos urbanos y rurales. Comerciantes, instituciones educativas, centros empresariales y entidades públicas requieren sistemas rápidos de alerta para notificar situaciones de emergencia (robos, agresiones, emergencias médicas). Actualmente, los sistemas de alarma convencionales no son lo suficientemente inmediatos o accesibles.

## 2. Planteamiento del problema
No existe una solución tecnológica práctica y de bajo costo que permita a una persona notificar de inmediato a las autoridades o personal de seguridad en caso de una emergencia. La ausencia de sistemas de botón de pánico confiables aumenta la vulnerabilidad de usuarios y negocios.

## 3. Stakeholders
- **Usuarios finales**: Comerciantes, estudiantes, personal de oficinas.
- **Autoridades**: Policía, entes de seguridad privada.
- **Entidades**: Alcaldías, empresas privadas que busquen implementar el sistema.
- **Equipo de desarrollo**: Product Owner, Scrum Master, desarrolladores.

## 4. Requisitos
### Requisitos funcionales
- El usuario puede activar una alarma con un clic en la aplicación o con un dispositivo físico (botón).
- El sistema envía una notificación inmediata a un panel central y a las autoridades definidas.
- Registro de incidentes en base de datos.
- Panel de administración para configurar usuarios, ubicaciones y zonas de alerta.

### Requisitos no funcionales
- Alta disponibilidad y estabilidad.
- Respuesta en menos de 3 segundos después de activar el botón.
- Interfaz sencilla y accesible.
- Escalabilidad para múltiples usuarios y entidades.

## 5. Historias de usuario (ejemplos)
- **HU-01**: Como comerciante, quiero presionar un botón de pánico para que la policía sea alertada en caso de robo.
- **HU-02**: Como estudiante, quiero acceder a una app en mi celular para enviar una alerta en una situación de peligro.
- **HU-03**: Como entidad de seguridad, quiero recibir un reporte con la ubicación exacta de la alerta para atender rápidamente la emergencia.

## 6. Diagrama de flujo (versión simplificada)
```mermaid
flowchart TD
    A[Usuario presiona botón] --> B[Se genera señal de alerta]
    B --> C[Servidor procesa alerta]
    C --> D[Notificación a autoridades]
    C --> E[Registro en base de datos]
    D --> F[Respuesta y acción de seguridad]
