# Casos de Uso Detallados para los Requisitos Funcionales
Todos los casos de uso están alineados con los estándares de la Ingeniería de Software, incluyendo actores, flujos y condiciones claras.
## RF1: Agendamiento de citas
### UC-001 – Agendar cita médica

### Actor Principal
Paciente

### Descripción
Permite al paciente seleccionar fecha, hora y tipo de consulta mediante una interfaz.
### Precondiciones:
1.	El paciente está autenticado en el sistema.
2.	Existen horarios disponibles para el psicólogo seleccionado.

#### 3. Flujo Principal:
4.	El paciente accede al módulo de agendamiento.
5.	El sistema muestra las fechas y horarios disponibles.
6.	El paciente selecciona fecha, hora y tipo de consulta.
7.	El sistema valida la disponibilidad.
8.	El paciente confirma la cita.
9.	El sistema registra la cita y muestra un mensaje de confirmación.
#### 10. Flujos Alternativos:
11.	**FA1:** No hay disponibilidad en la fecha/hora seleccionada.
12.	El sistema sugiere opciones alternativas.
13.	El paciente elige una nueva opción o cancela el proceso.
14.	**FA2:** Datos inválidos (ej. fecha pasada).
15.	El sistema muestra un mensaje de error y solicita corrección.

#### 16.	Postcondiciones:
17.	La cita queda registrada en el sistema.
18.	Se envía una notificación de confirmación al paciente (RF3).

## RF2: Gestión de citas por administradores
### UC-002 – Modificar/Reasignar/Cancelar citas

### Actor Principal
Administrador

### Descripción
Permite al administrador ajustar citas existentes.

### Precondiciones:
1.	La cita está registrada en el sistema.
2.	El administrador tiene permisos de gestión.
#### 3.	Flujo Principal:
4.	El administrador busca la cita por paciente o fecha.
5.	El sistema muestra los detalles de la cita.
6.	El administrador selecciona "Modificar", "Reasignar" o "Cancelar".
7.	El sistema valida la disponibilidad del psicólogo (si aplica).
8.	El administrador confirma los cambios.
9.	El sistema actualiza la cita y notifica al paciente (RF3).
#### 10.	Flujos Alternativos:
11.	**FA1:** El psicólogo reasignado no está disponible.
12.	El sistema muestra un error y sugiere otros profesionales.
#### 13.	Postcondiciones:
14.	La cita queda actualizada o cancelada.
15.	El paciente recibe una notificación del cambio (RF3).

## RF3: Notificaciones automáticas

### UC-003 – Enviar notificaciones de estado de citas
### Actor Principal
Sistema

### Descripción
El sistema envía alertas automáticas sobre confirmaciones, recordatorios, cambios o cancelaciones.

### Precondiciones:
1.	Existe una cita registrada o modificada.
2.	El paciente/administrador tiene datos de contacto válidos.
#### 3.	Flujo Principal:
4.	El sistema detecta un evento (ej. confirmación, cambio, cancelación).
5.	El sistema genera un mensaje con los detalles del evento.
6.	El sistema envía la notificación por correo electrónico o SMS.
7.	El sistema registra el envío en el historial.
#### 8.	Flujos Alternativos:
9.	**FA1:** Fallo en el envío.
10.	El sistema reintenta el envío después de 5 minutos.
11.	Si persiste el error, registra una alerta para el administrador.
#### 12.	Postcondiciones:
13.	El usuario recibe la notificación correspondiente.

## RF4: Registro de datos
### UC-004 – Gestionar datos socioeconómicos

### Actor Principal
Administrador
### Descripción
Permite registrar y actualizar datos socioeconómicos del paciente.

### Precondiciones:
1.	El paciente está registrado en el sistema.
#### 2.	Flujo Principal:
3.	El administrador accede al perfil del paciente.
4.	Selecciona "Datos Socioeconómicos".
5.	Ingresa información como ingresos, ocupación y dependientes.
6.	El sistema valida los campos obligatorios.
7.	El administrador guarda los datos.
#### 8.	Flujos Alternativos:
9.	**FA1:** Campos incompletos o inválidos.
10.	El sistema resalta los campos erróneos y solicita corrección.
#### 11. Postcondiciones:
12.	Los datos socioeconómicos quedan almacenados en el expediente.
