### **Caso de uso 1: Agendar cita inicial (vía web/App)**
**Actor principal**: Paciente.  
**Descripción**: El paciente agenda una cita inicial utilizando una plataforma digital (sitio web o app).  
**Precondiciones**:  
- El paciente tiene acceso a internet.  
- El sistema está disponible para recibir solicitudes.  

**Flujo principal**:  
1. El paciente accede al sistema y selecciona "Agendar cita".  
2. El sistema solicita datos personales básicos (nombre, teléfono, correo).  
3. El paciente ingresa la información.  
4. El sistema valida la disponibilidad de citas según el tipo de terapia requerida (Psicodiagnóstico, Clínica, etc.).  
5. El paciente selecciona fecha y hora disponibles.  
6. El sistema confirma la cita y genera un folio único.  
7. El sistema envía un comprobante automático al correo o WhatsApp del paciente.  
8. El paciente recibe un recordatorio 24 horas antes de la cita.  

**Flujos alternativos**:  
- Si el paciente no completa el proceso, el sistema envía un recordatorio por SMS para finalizar la acción.  
- Si no hay disponibilidad, el sistema ofrece registrar al paciente en una lista de espera.  
- Si el paciente no tiene correo electrónico, el sistema guarda el comprobante en su perfil para consulta posterior.  

**Postcondiciones**:  
- La cita queda registrada en el sistema.  
- El paciente recibe confirmación y recordatorio.  

---

### **Caso de uso 2: Agendar cita por teléfono**
**Actor principal**: Secretaria.  
**Descripción**: La secretaria registra una cita solicitada por un paciente vía telefónica.  
**Precondiciones**:  
- El paciente se comunica al número de la clínica (futuro, ya que actualmente no hay).  
- La secretaria tiene acceso al sistema.  

**Flujo principal**:  
1. El paciente llama para solicitar una cita.  
2. La secretaria ingresa al sistema y selecciona "Nueva cita por teléfono".  
3. La secretaria recopila los datos del paciente (nombre, teléfono, motivo de consulta).  
4. El sistema muestra las fechas disponibles según el tipo de terapia.  
5. La secretaria asigna una cita y confirma los detalles con el paciente.  
6. El sistema envía un SMS con el folio de la cita al paciente.  
7. La secretaria anota observaciones si el paciente requiere ajustes especiales.  

**Flujos alternativos**:  
- Si el paciente no responde al SMS de confirmación, la secretaria realiza una llamada de seguimiento.  
- Si el paciente proporciona datos incorrectos (ej: teléfono erróneo), el sistema marca la cita como "pendiente de validación".  

**Postcondiciones**:  
- La cita queda registrada en el sistema con el estatus "Confirmada".  
- El paciente recibe un SMS con los detalles.  

---

### **Caso de uso 3: Modificar una cita agendada**
**Actor principal**: Paciente o Secretaria.  
**Descripción**: El paciente o la secretaria ajustan la fecha/hora de una cita existente.  
**Precondiciones**:  
- La cita debe estar registrada en el sistema.  

**Flujo principal**:  
1. El paciente accede al sistema y selecciona "Modificar cita".  
2. El sistema solicita el folio de la cita.  
3. El paciente ingresa el folio y selecciona una nueva fecha/hora disponible.  
4. El sistema confirma el cambio y envía un correo/SMS con la actualización.  
5. Si la modificación afecta a otras sesiones (ej: tratamientos extensos), el sistema recalcula automáticamente el calendario.  

**Flujos alternativos**:  
- Si el paciente intenta modificar la cita menos de 24 horas antes, el sistema requiere aprobación de la secretaria.  
- Si la nueva fecha no está disponible, el sistema sugiere opciones alternas.  

**Postcondiciones**:  
- La cita se actualiza en el sistema.  
- El terapeuta asignado recibe una notificación del cambio.  

---

### **Caso de uso 4: Enviar recordatorio automático**
**Actor principal**: Sistema.  
**Descripción**: El sistema envía recordatorios de citas próximas para reducir inasistencias.  
**Precondiciones**:  
- La cita debe estar programada con al menos 24 horas de anticipación.  

**Flujo principal**:  
1. El sistema identifica las citas programadas para el día siguiente.  
2. Envía un mensaje (SMS/WhatsApp/correo) al paciente con:  
   - Fecha y hora de la cita.  
   - Nombre del terapeuta.  
   - Enlace para cancelar o reagendar.  
3. Si el paciente no confirma la recepción, el sistema notifica a la secretaria para seguimiento.  

**Flujos alternativos**:  
- Si el paciente marca "Cancelar" en el recordatorio, el sistema redirige al Caso de uso 3 (Modificar cita).  
- Si el mensaje falla (ej: número incorrecto), el sistema genera una alerta para la secretaria.  

**Postcondiciones**:  
- El paciente recibe el recordatorio.  
- Las inasistencias se reducen gracias a la confirmación proactiva.  

---

### **Caso de uso 5: Verificar disponibilidad en tiempo real**
**Actor principal**: Paciente o Secretaria.  
**Descripción**: Consultar las citas disponibles según el tipo de terapia y prioridad del paciente.  
**Precondiciones**:  
- El sistema debe tener actualizado el calendario de terapeutas.  

**Flujo principal**:  
1. El paciente/secretaria ingresa al sistema y selecciona "Ver disponibilidad".  
2. El sistema solicita:  
   - Tipo de terapia (Psicodiagnóstico, Clínica, etc.).  
   - Nivel de prioridad (según lista de espera).  
3. El sistema muestra un calendario con slots disponibles, resaltando las opciones más cercanas.  
4. Si el paciente tiene prioridad alta, el sistema sugiere fechas antes que a otros pacientes.  

**Flujos alternativos**:  
- Si no hay disponibilidad, el sistema muestra el tiempo estimado de espera y ofrece notificar cuando haya cupo.  
- Si la prioridad del paciente cambia (ej: urgencia), la secretaria puede ajustarla manualmente.  

**Postcondiciones**:  
- El paciente/secretaria conoce las opciones de agenda actualizadas.  

---

### **Caso de uso 6: Registrar datos socioeconómicos de manera virtual**
**Actor principal**: Paciente.  
**Descripción**: El paciente completa el formulario socioeconómico en línea antes de la cita.  
**Precondiciones**:  
- La cita debe estar agendada.  
- El paciente recibió un enlace seguro para completar el formulario.  

**Flujo principal**:  
1. El paciente accede al enlace proporcionado en el comprobante de la cita.  
2. El sistema muestra el formulario socioeconómico con campos obligatorios (ingresos, ocupación, etc.).  
3. El paciente completa y envía el formulario.  
4. El sistema valida que todos los campos estén llenos.  
5. Los datos se almacenan en el expediente del paciente.  
6. La secretaria revisa los datos y los marca como "Validados".  

**Flujos alternativos**:  
- Si el paciente no completa el formulario, el sistema envía recordatorios cada 24 horas.  
- Si hay inconsistencias (ej: ingresos no numéricos), la secretaria contacta al paciente para correcciones.  

**Postcondiciones**:  
- El formulario socioeconómico queda vinculado al expediente del paciente.  

---

### **Caso de uso 7: Manejar fallas en la comunicación**
**Actor principal**: Sistema y Secretaria.  
**Descripción**: Gestionar errores en el envío de notificaciones o recordatorios.  
**Precondiciones**:  
- El sistema detecta un fallo en la comunicación (ej: correo rebotado, SMS no entregado).  

**Flujo principal**:  
1. El sistema identifica un mensaje fallido y lo registra en un log de errores.  
2. Notifica a la secretaria con detalles del problema (ej: "Número inválido para el paciente X").  
3. La secretaria contacta al paciente por otro medio (ej: correo alternativo) para actualizar la información.  
4. Una vez corregidos los datos, el sistema reintenta el envío automáticamente.  

**Flujos alternativos**:  
- Si el paciente no responde a los intentos de contacto, la cita se marca como "Riesgo de inasistencia".  
- Si el error persiste (ej: servidor de correo caído), el sistema activa un protocolo de respaldo (ej: notificaciones por WhatsApp).  

**Postcondiciones**:  
- Los datos de contacto del paciente se actualizan.  
- La comunicación se restablece.  
