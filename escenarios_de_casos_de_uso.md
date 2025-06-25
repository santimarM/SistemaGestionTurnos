# Escenarios de Casos de Uso

---

## Caso de Uso 1: Registrar Paciente

- **ID Única:** CU001
- **Área:** Gestión de Pacientes
- **Actor(es):** Paciente
- **Descripción:** Permite a un nuevo paciente registrarse en el sistema para acceder a la solicitud de turnos.
- **Activar Evento:** El paciente accede a la opción “Registrarse” en el sistema.
- **Tipo de señal:** Externa (usuario inicia la acción)
- **Pasos desempeñados (ruta principal):**
  1. El paciente accede al formulario de registro.
  2. Completa sus datos personales: nombre, documento, fecha de nacimiento, teléfono, email.
  3. El sistema valida los datos.
  4. El sistema guarda el nuevo paciente.
  5. Se confirma el registro exitoso al paciente.
- **Precondiciones:** El paciente no debe estar previamente registrado.
- **Poscondiciones:** El paciente queda registrado en la base de datos.
- **Suposiciones:** El paciente cuenta con los datos requeridos y acceso al sistema.
- **Reunir requerimientos:** Formulario claro, validación obligatoria, feedback de éxito/error.
- **Aspectos sobresalientes:** ¿Cómo evitar duplicados? ¿Se envía correo de verificación?
- **Prioridad:** Alta
- **Riesgo:** Bajo

---

## Caso de Uso 2: Solicitar Turno

- **ID Única:** CU002
- **Área:** Gestión de Turnos
- **Actor(es):** Paciente
- **Descripción:** Permite al paciente solicitar un turno según la disponibilidad de médicos.
- **Activar Evento:** El paciente accede a la opción “Solicitar Turno”.
- **Tipo de señal:** Externa
- **Pasos desempeñados (ruta principal):**
  1. El paciente inicia sesión y accede a “Solicitar turno”.
  2. Elige especialidad y profesional.
  3. Selecciona fecha y hora disponible.
  4. Confirma el turno.
  5. El sistema registra el turno.
- **Precondiciones:** El paciente debe estar registrado e identificado.
- **Poscondiciones:** Turno asignado en estado “pendiente”.
- **Suposiciones:** Existe disponibilidad horaria.
- **Reunir requerimientos:** Agenda actualizada, validación simultánea.
- **Aspectos sobresalientes:** ¿Qué ocurre si dos pacientes eligen el mismo turno?
- **Prioridad:** Alta
- **Riesgo:** Medio

---

## Caso de Uso 3: Confirmar Turno

- **ID Única:** CU003
- **Área:** Gestión de Turnos
- **Actor(es):** Médico, Sistema
- **Descripción:** El médico confirma que atenderá un turno pendiente.
- **Activar Evento:** El médico accede a su agenda desde el sistema.
- **Tipo de señal:** Externa
- **Pasos desempeñados (ruta principal):**
  1. El médico inicia sesión.
  2. Visualiza la lista de turnos pendientes.
  3. Confirma uno o varios turnos.
  4. El sistema actualiza el estado a “confirmado”.
  5. Se notifica al paciente.
- **Precondiciones:** El turno debe estar en estado “pendiente”.
- **Poscondiciones:** El turno cambia a “confirmado”.
- **Suposiciones:** El médico tiene disponibilidad y acceso.
- **Reunir requerimientos:** Seguridad de acceso médico, notificaciones automáticas.
- **Aspectos sobresalientes:** ¿Qué pasa si el turno ya fue cancelado?
- **Prioridad:** Media
- **Riesgo:** Bajo

---

## Caso de Uso 4: Cancelar Turno

- **ID Única:** CU004
- **Área:** Gestión de Turnos
- **Actor(es):** Paciente
- **Descripción:** El paciente cancela un turno previamente solicitado.
- **Activar Evento:** El paciente accede a su listado de turnos.
- **Tipo de señal:** Externa
- **Pasos desempeñados (ruta principal):**
  1. El paciente inicia sesión.
  2. Selecciona un turno pendiente o confirmado.
  3. Hace clic en “Cancelar”.
  4. El sistema solicita confirmación.
  5. El turno se cancela y se actualiza su estado.
  6. Se notifica al médico.
- **Precondiciones:** Turno en estado “pendiente” o “confirmado”.
- **Poscondiciones:** El turno queda marcado como “cancelado”.
- **Suposiciones:** El paciente accede antes del horario del turno.
- **Reunir requerimientos:** Reglas para cancelación con tiempo mínimo.
- **Aspectos sobresalientes:** ¿Cuánto tiempo antes se puede cancelar?
- **Prioridad:** Alta
- **Riesgo:** Medio

---

## Caso de Uso 5: Consultar Historial

- **ID Única:** CU005
- **Área:** Historial Clínico
- **Actor(es):** Paciente
- **Descripción:** El paciente puede ver el listado de turnos pasados.
- **Activar Evento:** El paciente accede a “Historial de Turnos”.
- **Tipo de señal:** Externa
- **Pasos desempeñados (ruta principal):**
  1. El paciente inicia sesión.
  2. Accede al historial desde el menú.
  3. El sistema muestra los turnos pasados (fecha, médico, estado, motivo).
- **Precondiciones:** El paciente debe haber tenido turnos anteriores.
- **Poscondiciones:** Visualización del historial completo.
- **Suposiciones:** La base de datos guarda el historial sin errores.
- **Reunir requerimientos:** Filtros por fecha, estado, especialidad.
- **Aspectos sobresalientes:** ¿Se pueden exportar los datos? ¿Se ven observaciones?
- **Prioridad:** Media
- **Riesgo:** Bajo


