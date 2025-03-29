# Especificación de requerimientos de software

## Requerimientos Funcionales
Gestión de citas y consultas
| ID | Nombre | Descripción |
| -- | ------ | ----------- |
| RF1 | Agendamiento de citas | El sistema debe permitir a los pacientes agendar citas médicas seleccionando fecha, hora y tipo de consulta a través de una interfaz. |
| RF2 | Gestión de citas por administradores. | Los administradores pueden modificar, reasignar o cancelar citas de los pacientes, garantizando la disponibilidad del personal de los psicólog(a)s. |
| RF3 | Notificaciones automáticas. | El sistema debe enviar notificaciones automáticas sobre el estado de las citas, incluyendo confirmación, recordatorios, cambios de horario o cancelaciones en dado de existir. |
| RF4 | Almacenamiento de datos de pacientes. | El sistema debe permitir registrar y administrar la información personal y de contacto de los pacientes, asegurando la integridad y seguridad de los datos. |
| RF5 | Consulta de historial de citas | Los administradores pueden acceder al historial completo de citas de cada paciente, incluyendo detalles de las consultas previas y las próximas. |
| RF6 | Registro de datos socioeconómicos. | El sistema cuenta con un módulo que permita registrar y gestionar los datos socioeconómicos de los pacientes, los cuales podrán ser utilizados para evaluación de subsidios o beneficios. |
| RF7 | Genración de reportes. | El sistema debe generar reportes diarios estadísticos sobre las citas agendadas, canceladas y atendidas, permitiendo filtrar por fechas, profesionales y tipos de consulta. |

### Criterios de validación para requerimientos funcionales.
Ver documento relacionado: [Criterios de Validacion Requerimientos Funcionales](Criterios_Validacion_Funcionales.md)
## Requerimientos No Funcionales

### Experiencia y Usabilidad

| ID | Nombre | Descripción |
| -- | ------ | ----------- |
| RNF1 | Interfaz intuitiva. | El sistema ofrece una interfaz gráfica sencilla y fácil de usar para el personal administrativo. |
| RNF2 | Interfaz adaptable. | El sistema debe tener una interfaz que debe adaptarse automáticamente a diferentes resoluciones de pantalla sin perder funcionalidad. |
| RNF3 | Accesibilidad en la infraestructura. |El sistema debe ser accesible desde los distintos dispositivos de la oficina administrativa y funcionar correctamente en ellos durante todo el tiempo de utilidad. |

### Accesibilidad

| ID | Nombre | Descripción |
| -- | ------ | ----------- |
| RNF5 | Contrastes visuales | El sistema debe contar con contraste y tamaño de texto siguiendo practicas de accesibilidad para facilitar la lectura. |

### Criterios de validación para requerimientos no funcionales.
Ver documento relacionado: [Criterios de Validacion Requerimientos No Funcionales](Criterios_Validacion_No_Funcionales.md)


## Casos de uso

Se identificaron 6 Casos de uso en el sistema:
1. Agendar cita médica.
2. Modificar/Reasignar/Cancelar citas.
3. Enviar notificaciones de estado de citas.
4. Acceder al historial clínico.
5. Gestionar datos socioeconómicos.
6. Generar reporte estadístico.

Para mayor detalle de cada caso de uso, consulte el documento relacionado [Casos de Uso](Casos_De_Uso.md).
