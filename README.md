# Prototipo del sistema de la  clinica de psicología

## Sistema de Gestión Administrativa para la Clínica de Psicología UADY

Este proyecto aborda la necesidad de modernizar la gestión en la clínica de la Facultad de Psicología de la UADY, la cual ofrece servicios de psicodiagnóstico y psicoterapia. Actualmente, todos los procesos, desde el agendamiento inicial de citas para recopilación de información hasta la calendarización y control de pagos, se realizan manualmente en papel. Esta metodología es ineficiente y genera dificultades en el control, la búsqueda de información y la reprogramación de citas, entre otros procesos.

El **Sistema de Gestión Administrativa** propuesto busca solucionar esta problemática. Para esta **Tercera Entrega**, nuestro equipo se ha centrado específicamente en el primer contacto entre la clínica y los posibles pacientes. El enfoque principal es la **optimización de la programación de citas para la recopilación de datos y la realización del estudio socioeconómico de los posibles pacientes**.



El objetivo general del sistema a largo plazo es:
* Automatizar el registro de citas, eliminando el proceso manual y reduciendo errores.
* Mejorar la comunicación mediante la implementación de recordatorios automáticos para pacientes y notificaciones para el personal.
* Facilitar las tareas del personal administrativo y los profesionales de la clínica, mejorando también la experiencia del paciente.

Te invitamos a explorar el contenido de esta entrega para conocer en detalle el trabajo realizado en la búsqueda de una solución eficiente y sencilla para el departamento de administración de la clínica.

## Requisitos Funcionales

Gestión de citas y consultas
| ID | Nombre | Descripción |
| -- | ------ | ----------- |
| RF1 | Agendamiento de citas | El sistema debe permitir a los pacientes agendar citas médicas seleccionando fecha, hora y tipo de consulta a través de una interfaz. |
| RF2 | Notificaciones automáticas. | El sistema debe enviar notificaciones automáticas sobre el estado de las citas, incluyendo confirmación, recordatorios, cambios de horario o cancelaciones en dado de existir. |
| RF3 | Registro de datos. | El sistema cuenta con un módulo que permita registrar y gestionar los datos de los pacientes que la secretaria/administrador obtiene durante el primer contacto, los cuales podrán ser utilizados para evaluación de pasos posteriores. |


### Criterios de validación para requerimientos funcionales.
Ver documento relacionado: [Criterios de Validacion Requerimientos Funcionales](ERS/Criterios_Validacion_Funcionales.md)
## Requerimientos No Funcionales

### Experiencia y Usabilidad

| ID | Nombre | Descripción |
| -- | ------ | ----------- |
| RNF1 | Interfaz intuitiva. | El sistema ofrece una interfaz gráfica sencilla y fácil de usar para el personal administrativo. |
| RNF2 | Interfaz adaptable. | El sistema debe tener una interfaz que debe adaptarse automáticamente a diferentes resoluciones de pantalla sin perder funcionalidad. |
| RNF3 | Accesibilidad en la infraestructura. |El sistema debe ser accesible desde los distintos dispositivos de la oficina administrativa y funcionar correctamente en ellos durante todo el tiempo de utilidad. |

### Criterios de validación para requerimientos no funcionales.
Ver documento relacionado: [Criterios de Validacion Requerimientos No Funcionales](ERS/Criterios_Validacion_No_Funcionales.md)


## Casos de uso

Se identificaron 4 Casos de uso en el sistema:
1. Agendar cita médica.
2. Modificar/Reasignar/Cancelar citas.
3. Enviar notificaciones de estado de citas.
4. Capturar datos.

Para mayor detalle de cada caso de uso, consulte el documento relacionado [Casos de Uso](ERS/Casos_De_Uso.md).


## Prototipado de interfaces

##### Página principal

[![Captura-de-pantalla-2025-05-29-110718.png](https://i.postimg.cc/dQhgRdhY/Captura-de-pantalla-2025-05-29-110718.png)](https://postimg.cc/9zjxCDP8)

#### Formulario de solicitud de cita

[![Captura-de-pantalla-2025-05-30-160510.png](https://i.postimg.cc/V6KvzJm8/Captura-de-pantalla-2025-05-30-160510.png)](https://postimg.cc/cg80m4v9)

#### Confirmación de solicitud de citas

[![Captura-de-pantalla-2025-05-30-160805.png](https://i.postimg.cc/T1Y6Y0Q7/Captura-de-pantalla-2025-05-30-160805.png)](https://postimg.cc/xJ776KwM)

#### Consulta de citas

[![Captura-de-pantalla-2025-05-30-161842.png](https://i.postimg.cc/6q4n1kGn/Captura-de-pantalla-2025-05-30-161842.png)](https://postimg.cc/5Q1XXkg2)

[![Captura-de-pantalla-2025-05-30-162025.png](https://i.postimg.cc/VNyfj3z2/Captura-de-pantalla-2025-05-30-162025.png)](https://postimg.cc/CRNp0rB4)

#### Cancelación de citas

[![Captura-de-pantalla-2025-05-30-162245.png](https://i.postimg.cc/441QjgMb/Captura-de-pantalla-2025-05-30-162245.png)](https://postimg.cc/fkJd06MJ)

[![Captura-de-pantalla-2025-05-30-162339.png](https://i.postimg.cc/Qtsg48Q7/Captura-de-pantalla-2025-05-30-162339.png)](https://postimg.cc/NyJrLwPG)

### Colaboradores

- **Marco Santiago Canché May** - Product Owner / Developer
  [[Github]](https://github.com/MarcoSIIIU)
  [[LinkedIn]]((https://www.linkedin.com/in/marcocanchemscm/))

- **Gabriel Sanchez Peraza** - Scrum master / Developer
  [[Github]](https://github.com/GabSPz)
  [[LinkedIn]](https://www.linkedin.com/in/gabriel-sanchez-peraza-21b59a248/)

- **José Luis Gutiérrez Couoh** - Developer
[[Github]](https://github.com/Josegutierrezcouoh)
[[LinkedIn]](https://www.linkedin.com/in/josé-gutiérrez-96a3bb28b/)

- **Fernando Canul Caballero** - Developer
[[Github]](https://github.com/elegidocodes)
[[LinkedIn]](https://www.linkedin.com)

- **Victor Hugo Rosado** - Developer
[[Github]](https://github.com/VictorHugoRok)
[[LinkedIn]](https://www.linkedin.com)



