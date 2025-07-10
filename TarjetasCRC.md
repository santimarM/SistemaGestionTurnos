# Tarjetas CRC – Sistema de Gestión de Turnos Médicos

---

## Clase: Paciente

### Superclase:
Usuario

### Subclase:
*(No definida)*

### Responsabilidades y Detalles

| Responsabilidad                         | Colaboradores | Pensamiento del objeto                                                | Propiedad      |
|-----------------------------------------|---------------|------------------------------------------------------------------------|----------------|
| Consultar turnos                        | GestorTurnos  | Conozco mis turnos pasados y próximos                                  | historialTurnos |
| Solicitar turno médico                  | GestorTurnos  | Sé qué especialidad necesito y qué fechas tengo disponibles            | dni            |
| Cancelar un turno                       | GestorTurnos  | Puedo identificar el turno que quiero cancelar                         | nombreApellido |

---

## Clase: Médico

### Superclase:
Usuario

### Subclase:
*(No definida)*

### Responsabilidades y Detalles

| Responsabilidad                         | Colaboradores | Pensamiento del objeto                                           | Propiedad       |
|-----------------------------------------|---------------|------------------------------------------------------------------|-----------------|
| Visualizar historial médico del paciente| Sistema       | Necesito ver los turnos y diagnósticos anteriores                | matricula       |
| Atender al paciente                     | Paciente      | Puedo generar observaciones o diagnósticos en la consulta         | especialidad    |
| Confirmar asistencia a turno            | Sistema       | Verifico si el paciente se presentó al turno asignado            | nombreApellido  |

---

## Clase: Turno

### Superclase:
*(No definida)*

### Subclase:
*(No definida)*

### Responsabilidades y Detalles

| Responsabilidad                 | Colaboradores | Pensamiento del objeto                                | Propiedad    |
|--------------------------------|---------------|--------------------------------------------------------|--------------|
| Asociar paciente con médico    | Paciente, Médico | Puedo guardar la relación entre un paciente y un médico | fecha        |
| Registrar horario y especialidad | Médico        | Tengo una hora y una especialidad asignada             | hora         |
| Permitir cancelación           | Paciente       | Puedo ser cancelado antes de que se cumpla mi fecha     | estado       |

---

## Clase: GestorTurnos

### Superclase:
*(No definida)*

### Subclase:
*(No definida)*

### Responsabilidades y Detalles

| Responsabilidad                         | Colaboradores | Pensamiento del objeto                                            | Propiedad         |
|-----------------------------------------|---------------|-------------------------------------------------------------------|-------------------|
| Registrar nuevo turno                   | Paciente, Médico | Tomo los datos del paciente y médico y creo un nuevo turno         | turnosProgramados |
| Cancelar turno existente                | Paciente      | Puedo encontrar y eliminar un turno si el paciente lo solicita     | turnosProgramados |
| Verificar disponibilidad del médico     | Médico        | Accedo a la agenda del médico para ver si tiene horarios libres    | agendaMedica      |

