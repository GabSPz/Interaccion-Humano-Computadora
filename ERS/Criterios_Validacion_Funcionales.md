# Criterios de Validación para los Requerimientos Funcionales.

**Propósito**: El propósito del documento es dar algunos criterios recomendables para la validación de los requerimientos funcionales especificados previamente en una parte del sistema de gestión de citas de la facultad de psicología.

## RF1 - Agendamiento de citas

### Descripción del Criterio
 El sistema debe permitir a los pacientes seleccionar fecha, hora y tipo de consulta a través de una interfaz de usuario.

### Condiciones de Aceptación
1.	El paciente puede visualizar un calendario con la disponibilidad de horarios.
2.	Se valida que la fecha y hora seleccionadas estén disponibles.
3.	Se almacena la cita en la base de datos.
4.	Se muestra la cita en el historial del paciente.
5.	Se genera una confirmación de la cita (correo electrónico o notificación en la plataforma).

### Método de Validación
 * Prueba funcional agendando una cita desde la interfaz de usuario.
 * Validación de registros en la base de datos para verificar que la cita fue almacenada correctamente.


## RF2 – Gestión de citas por administradores

### Descripción del Criterio
Los administradores deben poder modificar, reasignar o cancelar citas según disponibilidad.

### Condiciones de Aceptación
1.	Un administrador puede visualizar la lista de citas programadas.
2.	Puede modificar la fecha, hora o profesional de una cita.
3.	El sistema verifica que la nueva fecha y hora estén disponibles antes de aceptar la modificación.
4.	Si se cancela una cita, se elimina del historial activo y se notifica al paciente.

### Método de Validación
 * Prueba funcional en la interfaz de administración, modificando y cancelando citas.
 * Validación en la base de datos de cambios en las citas.
 * Prueba de notificación de modificación/cancelación.

## RF3 – Notificaciones automáticas

### Descripción del Criterio
El sistema debe enviar notificaciones automáticas sobre cambios en sus citas.

### Condiciones de Aceptación
1.	Se recibe una notificación cuando agenda una cita.
2.	Se envía un recordatorio automático 24 horas antes de la cita.
3.	Si la cita es modificada o cancelada, el paciente recibe una notificación con los detalles.
4.	Las notificaciones pueden enviarse por correo electrónico o mensaje en la plataforma.
5.	Se debe registrar un historial de notificaciones enviadas.

### Método de Validación
 * Prueba funcional agendando, modificando y cancelando citas para verificar la recepción de notificaciones.
 * Revisión del historial de notificaciones en la base de datos.

## RF4 – Almacenamiento de datos de pacientes

### Descripción del Criterio
El sistema debe registrar y administrar la información personal de los pacientes de manera segura.
### Condiciones de Aceptación
1.	Se permite registrar nuevos pacientes con nombre, contacto y datos personales.
2.	La información del paciente debe almacenarse en una base de datos encriptada.
3.	Solo los usuarios autorizados pueden acceder a la información del paciente.
4.	Los datos personales deben ser editables únicamente por personal autorizado.
### Método de Validación
 * Pruebas funcionales creando y editando registros de pacientes.
 * Prueba de acceso restringido (usuarios no autorizados no deben ver ni modificar datos).
 * Revisión de la encriptación de datos en la base de datos.

## RF5 – Consulta del historial de citas

### Descripción del Criterio
Los administradores pueden consultar el historial completo de citas de cada paciente.
### Condiciones de Aceptación
1.	Un administrador puede seleccionar a un paciente y visualizar su historial de citas.
2.	Se muestran detalles como fecha, hora, profesional y estado de la cita.
3.	Solo los usuarios autorizados pueden acceder a esta información.
4.	El historial debe ser actualizado en tiempo real con cada nueva cita o modificación.
### Método de Validación:
 * Prueba funcional de consulta del historial de un paciente en la interfaz de administración.
 * Prueba de acceso restringido.

## RF6 – Registro de datos socioeconómicos
### Descripción del Criterio
El sistema debe permitir registrar y administrar datos socioeconómicos de los pacientes.

### Condiciones de Aceptación
1.	Un administrador puede ingresar datos sobre nivel socioeconómico, ingresos, escolaridad, etc.
2.	La información debe poder ser modificada solo por personal autorizado.
3.	Los datos deben almacenarse de manera segura y ser accesibles solo para análisis.
4.	Se debe permitir la generación de reportes basados en esta información.

### Método de Validación
 * Pruebas funcionales de ingreso y consulta de datos socioeconómicos.
 * Generación de reportes de prueba para validar la correcta captura de información.

## RF7 – Generación de reportes
### Descripción del Criterio
El sistema debe generar reportes sobre citas agendadas, canceladas y atendidas.

### Condiciones de Aceptación
1.	Se puede seleccionar un rango de fechas para generar reportes.
2.	Se puede filtrar por profesional, estado de la cita y tipo de consulta.
3.	Los reportes deben mostrarse en pantalla y permitir exportación a PDF o Excel.
4.	Solo los administradores pueden acceder a la generación de reportes.

### Método de Validación:
 * Prueba funcional generando reportes con distintos filtros.
 * Verificación de exportación de reportes a distintos formatos.
 * Prueba de acceso restringido a la funcionalidad de reportes.
