# Escenarios de Casos de Uso

A continuación se presentan los diferentes escenarios derivados de cada caso de uso, siguiendo el formato: "Caso de Uso – Nombre del Escenario".

---

### Caso de Uso 1 – Registrar Paciente 

## Escenario 1 - Registro exitoso de nuevo paciente ##

-  Actor: Recepcionista  
- Precondición: El paciente no debe estar registrado.  
-  Flujo:
  1. El recepcionista accede al formulario de registro.
  2. Ingresa todos los datos requeridos del paciente correctamente.
  3. El sistema valida la información.
  4. El sistema guarda el nuevo paciente.
-  Postcondición: El paciente queda registrado en el sistema.

---

## Escenario 2 - Registrar Paciente – Error en validación de datos del paciente

-  Actor: Recepcionista  
-  Precondición: El paciente no debe estar registrado.  
-  Flujo:
  1. El recepcionista accede al formulario.
  2. Ingresa datos incompletos o mal formateados (por ejemplo, un DNI inválido).
  3. El sistema detecta el error y muestra un mensaje.
  4. El sistema no permite continuar hasta corregir los errores.
-  Postcondición: El paciente no se registra.

---

##Escenario 3 - Registrar Paciente – Paciente ya registrado

-  Actor: Recepcionista  
-  Precondición: El paciente ya existe en la base de datos.  
-  Flujo:
  1. El recepcionista intenta registrar un nuevo paciente con un DNI que ya está registrado.
  2. El sistema detecta la duplicación.
  3. El sistema muestra un mensaje de advertencia.
  4. El sistema no guarda al paciente nuevamente.
-  Postcondición: El sistema mantiene la información original sin duplicar datos.

---

### Caso de Uso 2 – Asignar Turno 

##Escenario 1 - Turno asignado exitosamente

-  Actor: Paciente / Recepcionista  
-  Precondición: El paciente está registrado y el médico tiene disponibilidad.  
-  Flujo:
  1. El paciente o recepcionista accede al módulo de asignación de turnos.
  2. Selecciona médico, especialidad, fecha y hora.
  3. El sistema verifica la disponibilidad.
  4. El sistema guarda el turno.
-  Postcondición: Turno registrado y confirmado.

---

##Escenario 2 -  Asignar Turno – Médico sin disponibilidad

- Actor: Paciente / Recepcionista  
-  Precondición: El paciente está registrado.  
-  Flujo:
  1. El paciente o recepcionista selecciona un médico y una fecha.
  2. El sistema verifica y detecta que no hay horarios disponibles ese día.
  3. El sistema informa al usuario.
  4. El sistema permite seleccionar otra fecha u otro médico.
-  Postcondición: El turno no se registra.

---

##Escenario 3 - Asignar Turno – Paciente no registrado

-  Actor: Paciente / Recepcionista  
- Precondición: El paciente no está en el sistema.  
- Flujo:
  1. El paciente solicita un turno.
  2. El sistema intenta validar sus datos.
  3. Detecta que el paciente no existe.
  4. Informa al recepcionista que debe registrarlo primero.
-  Postcondición: No se asigna el turno.

---

### Caso de Uso 3 – Cancelar Turno 

##Escenario 1 - Cancelación exitosa por paciente

-  Actor: Paciente  
-  Precondición: El paciente tiene un turno previamente registrado.  
-  Flujo:
  1. El paciente accede al sistema.
  2. Selecciona el turno que desea cancelar.
  3. Confirma la acción.
  4. El sistema cambia el estado del turno a "Cancelado".
-  Postcondición: El turno queda cancelado correctamente.

---

##Escenario 2 - Cancelar Turno – Cancelación por parte del médico

-  Actor: Médico  
-  Precondición: El médico tiene un turno asignado con un paciente.  
-  Flujo:
  1. El médico accede a su agenda.
  2. Marca un turno como cancelado (por ausencia o motivo personal).
  3. El sistema actualiza el estado del turno.
  4. Se notifica al paciente del cambio.
-  Postcondición: El turno se cancela y se genera una notificación.

---

##Escenario 3 -  Cancelar Turno – Intento de cancelación de turno inexistente

-  Actor: Paciente / Recepcionista  
-  Precondición: El turno seleccionado no existe o ya fue cancelado previamente.  
-  Flujo:
  1. El actor accede al sistema y selecciona un turno.
  2. El sistema no encuentra un turno válido con ese ID o ya cancelado.
  3. Se informa al usuario del error.
-  Postcondición: No se realiza ninguna acción.

---

### Caso de Uso 4 – Consultar Historial Médico 

##Escenario 1 – Visualización exitosa

-  Actor: Médico  
-  Precondición: El médico está autenticado y el paciente está registrado.  
-  Flujo:
  1. El médico inicia sesión en el sistema.
  2. Selecciona un paciente de su lista.
  3. El sistema muestra el historial clínico completo del paciente.
-  Postcondición: El historial es visualizado correctamente.

---

##Escenario 2 - Consultar Historial Médico - Paciente sin historial

-  Actor: Médico  
-  Precondición: El paciente está registrado pero nunca tuvo turnos.  
-  Flujo:
  1. El médico busca al paciente.
  2. El sistema informa que no existen registros médicos previos.
  3. El sistema permite seguir con nuevas entradas.
-  Postcondición: No se muestra historial, pero se habilita el registro futuro.

---

##Escenario 3 -  Consultar Historial Médico - Médico no autenticado

-  Actor: Médico  
-  Precondición: El usuario no ha iniciado sesión.  
-  Flujo:
  1. El médico intenta acceder al historial.
  2. El sistema detecta que no hay sesión activa.
  3. El sistema redirige a la pantalla de inicio de sesión.
-  Postcondición: El historial no es mostrado.

---

## Caso de Uso 5 – Registrar Médico 

##Escenario 1 - – Registro exitoso

- Actor: Recepcionista  
- Precondición: El recepcionista está autenticado en el sistema.  
- Flujo:
  1. El recepcionista accede a la opción “Registrar Médico”.
  2. El sistema muestra el formulario de registro.
  3. El recepcionista ingresa nombre, apellido, especialidad, matrícula, teléfono.
  4. El sistema valida los datos ingresados.
  5. La matrícula no está registrada.
  6. El sistema registra al nuevo médico y confirma el alta.  
- Postcondición: El médico queda registrado correctamente en el sistema.

---

##Escenario 2 -  Registrar Médico – Matrícula ya registrada

- Actor: Recepcionista  
- Precondición: El recepcionista está autenticado y existe un médico con esa matrícula.  
- Flujo:
  1. El recepcionista accede al formulario de “Registrar Médico”.
  2. Ingresa los datos, incluyendo una matrícula ya existente.
  3. El sistema valida los datos y detecta duplicado.
  4. Se informa al recepcionista que la matrícula ya está registrada.
  5. El sistema solicita cambiar la matrícula.  
- Postcondición: El médico no es registrado y se evita duplicación.

---

##Escenario 3 – Registrar Médico – Recepcionista no autenticado

- Actor: Recepcionista  
- Precondición: El usuario no inició sesión.  
- Flujo:
  1. El recepcionista intenta acceder a la opción “Registrar Médico”.
  2. El sistema detecta que no hay sesión activa.
  3. El sistema redirige a la pantalla de login.  
- Postcondición: El formulario de registro no es accesible sin autenticación.

