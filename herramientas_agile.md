**Tarjeta CRC 1: Paciente**

- Nombre de la clase: Paciente
- Superclase: Persona
- Subclase: Ninguna
- Pensamiento del objeto: Representa a un paciente que se registra en el sistema y solicita turnos con profesionales de la salud.
- Responsabilidades principales:
- Registrar información personal
- Solicitar turnos con profesionales de la salud
- Verificar disponibilidad de turnos
- Colaboraciones con otras clases:
- ProfesionalDeLaSalud
- Turno
- Propiedad a la que se referenciará: Identificador de paciente, nombre, fecha de nacimiento, dirección, teléfono.

**Tarjeta CRC 2: ProfesionalDeLaSalud**

- Nombre de la clase: ProfesionalDeLaSalud
- Superclase: Persona
- Subclase: Médico, Enfermero, etc.
- Pensamiento del objeto: Representa a un profesional de la salud que atiende a pacientes y tiene turnos asignados.
- Responsabilidades principales:
- Atender a pacientes
- Asignar turnos
- Verificar disponibilidad de turnos
- Colaboraciones con otras clases:
- Paciente
- Turno
- Propiedad a la que se referenciará: Identificador de profesional, nombre, especialidad, horario de atención.

**Tarjeta CRC 3: Turno**

- Nombre de la clase: Turno
- Superclase: Ninguna
- Subclase: Ninguna
- Pensamiento del objeto: Representa un turno asignado a un paciente con un profesional de la salud.
- Responsabilidades principales:
- Asignar turno a un paciente
- Verificar disponibilidad de turnos
- Cancelar turno
- Colaboraciones con otras clases:
- Paciente
- ProfesionalDeLaSalud
- Propiedad a la que se referenciará: Identificador de turno, fecha, hora, paciente, profesional de la salud.

**Tarjeta CRC 4: RegistroDeTurnos**

- Nombre de la clase: RegistroDeTurnos
- Superclase: Ninguna
- Subclase: Ninguna
- Pensamiento del objeto: Representa un registro de todos los turnos asignados y realizados.
- Responsabilidades principales:
- Registrar turnos
- Verificar historial de turnos
- Colaboraciones con otras clases:
- Turno
- Paciente
- ProfesionalDeLaSalud
- Propiedad a la que se referenciará: Identificador de registro, lista de turnos.

**Tarjeta CRC 5: Notificación**

- Nombre de la clase: Notificación
- Superclase: Ninguna
- Subclase: NotificaciónDeTurno, NotificaciónDeCancelación, etc.
- Pensamiento del objeto: Representa una notificación enviada a un paciente o profesional de la salud.
- Responsabilidades principales:
- Enviar notificación
- Verificar tipo de notificación
- Colaboraciones con otras clases:
- Paciente
- ProfesionalDeLaSalud
- Turno
- Propiedad a la que se referenciará: Identificador de notificación, tipo de notificación, mensaje.
