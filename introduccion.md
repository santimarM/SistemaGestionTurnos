# **Introducción**


# **Descripción del paradigma orientado a objetos**

La Programación Orientada a Objetos (POO) es un paradigma de programación que se basa en la idea de que los programas se pueden diseñar y estructurar alrededor de objetos que interactúan entre sí. Estos objetos representan entidades del mundo real y tienen propiedades y comportamientos que se pueden definir y manipular.

# **Importancia de la POO**

La POO es importante porque permite:

- Crear programas más modulares y reutilizables
- Modelar sistemas complejos de manera más natural y intuitiva
- Reducir la complejidad del código y mejorar su mantenibilidad

  
 **Los cuatro fundamentos de la POO**

 **Encapsulamiento**

El encapsulamiento es un concepto fundamental en la Programación Orientada a Objetos (POO) que se refiere a la idea de ocultar los detalles internos de un objeto y exponer solo la información necesaria para interactuar con él

**Beneficios del encapsulamiento**

El encapsulamiento proporciona varios beneficios, incluyendo:

- Protección de la integridad de los datos: Al controlar el acceso a los datos, se evita que se realicen operaciones no válidas o que se acceda a información sensible de manera no autorizada.
- Mejora de la seguridad: Al ocultar los detalles internos de un objeto, se reduce el riesgo de que se exploten vulnerabilidades o se acceda a información confidencial.
- Mayor flexibilidad y mantenibilidad: Al proporcionar una interfaz clara y controlada para interactuar con un objeto, se facilita la modificación o extensión del objeto sin afectar a otros componentes del sistema.

 **Herencia**

La herencia es un concepto fundamental en la Programación Orientada a Objetos (POO) que permite crear nuevos objetos a partir de objetos existentes, heredando sus propiedades y comportamientos.

**Beneficios de la Herencia**

La herencia permite:

- Reutilizar código existente
- Crear jerarquías de clases naturales
- Especializar objetos en subclases
- Mayor flexibilidad y mantenibilidad

**Polimorfismo**
El polimorfismo es la capacidad de un objeto de tomar diferentes formas y comportamientos dependiendo del contexto en el que se utilice.

 **Beneficios Polimorfismo**

- Mayor flexibilidad y reutilización de código
- Permite tratar objetos de diferentes clases de manera uniforme
- Facilita la creación de programas más genéricos y adaptables

**Abstracción**

La abstracción es la capacidad de enfocarse en los aspectos esenciales de un objeto o sistema y ignorar los detalles irrelevantes.

 **Beneficios Abstracción**

- Simplifica la complejidad de los sistemas
- Permite enfocarse en los aspectos importantes
- Facilita la comprensión y el análisis de los sistemas

 # **Requisitos Funcionales del Sistema de Gestión de Turnos Médicos**

 A continuación, se presentan cinco requisitos funcionales clave para el sistema de gestión de turnos médicos:

**1. Registro de Pacientes y Profesionales**
- El sistema debe permitir registrar información de pacientes y profesionales de la salud, incluyendo datos de contacto y detalles relevantes.

**2. Asignación de Turnos**
- El sistema debe permitir asignar turnos a pacientes con profesionales de la salud específicos, teniendo en cuenta la disponibilidad de los profesionales y los horarios de atención.

**3. Gestión de Turnos**
- El sistema debe permitir gestionar turnos, incluyendo la capacidad de:
- Verificar la disponibilidad de turnos
- Reservar turnos
- Cancelar turnos
- Modificar turnos

**4. Notificaciones y Alertas**
- El sistema debe enviar notificaciones y alertas a pacientes y profesionales de la salud sobre:
- Confirmación de turnos
- Cancelación de turnos
- Modificación de turnos

**5. Historial de Turnos**
- El sistema debe mantener un registro histórico de turnos asignados y realizados, permitiendo a los profesionales de la salud y pacientes acceder a información sobre turnos anteriores.

Estos requisitos funcionales son fundamentales para garantizar que el sistema de gestión de turnos médicos sea efectivo y eficiente en la gestión de la atención médica.

# **Casos de Uso del Sistema de Gestión de Turnos Médicos**

# **Caso de Uso 1: Registrar Paciente**

- Nombre del caso de uso: Registrar Paciente
- Actor(es) involucrado(s): Recepcionista
- Descripción breve: Registrar información de un paciente nuevo en el sistema.
- Flujo principal de eventos:
1. Ingresar al sistema y seleccionar "Registrar Paciente".
2. Ingresar información del paciente.
3. Verificar y confirmar la información.
4. Registrar al paciente en el sistema.
- Precondiciones: La recepcionista debe tener acceso al sistema.
- Postcondiciones: El paciente está registrado en el sistema.

# **Caso de Uso 2: Asignar Turno**

- Nombre del caso de uso: Asignar Turno
- Actor(es) involucrado(s): Recepcionista
- Descripción breve: Asignar un turno a un paciente con un profesional de la salud específico.
- Flujo principal de eventos:
1. Ingresar al sistema y seleccionar "Asignar Turno".
2. Seleccionar paciente y profesional de la salud.
3. Asignar turno y confirmar.
4. Enviar notificación al paciente y al profesional de la salud.
- Precondiciones: El paciente y el profesional de la salud deben estar registrados en el sistema.
- Postcondiciones: El turno está asignado y se envió una notificación.

# **Caso de Uso 3: Verificar Disponibilidad de Turnos**

- Nombre del caso de uso: Verificar Disponibilidad de Turnos
- Actor(es) involucrado(s): Paciente, Recepcionista
- Descripción breve: Verificar la disponibilidad de turnos para un profesional de la salud específico.
- Flujo principal de eventos:
1. Ingresar al sistema y seleccionar "Verificar Disponibilidad de Turnos".
2. Seleccionar profesional de la salud y fecha.
3. Verificar disponibilidad de turnos.
- Precondiciones: El profesional de la salud debe estar registrado en el sistema.
- Postcondiciones: Se muestra la disponibilidad de turnos.

# **Caso de Uso 4: Cancelar Turno**

- Nombre del caso de uso: Cancelar Turno
- Actor(es) involucrado(s): Recepcionista, Paciente
- Descripción breve: Cancelar un turno asignado.
- Flujo principal de eventos:
1. Ingresar al sistema y seleccionar "Cancelar Turno".
2. Seleccionar turno a cancelar.
3. Confirmar cancelación.
4. Enviar notificación al paciente y al profesional de la salud.
- Precondiciones: El turno debe estar asignado y no haber sido realizado.
- Postcondiciones: El turno está cancelado y se envió una notificación.

# **Caso de Uso 5: Ver Historial de Turnos**

- Nombre del caso de uso: Ver Historial de Turnos
- Actor(es) involucrado(s): Paciente, Profesional de la Salud
- Descripción breve: Ver el historial de turnos asignados y realizados.
- Flujo principal de eventos:
1. Ingresar al sistema y seleccionar "Ver Historial de Turnos".
2. Ver historial de turnos.
- Precondiciones: El paciente o el profesional de la salud debe estar registrado en el sistema.
- Postcondiciones: Se muestra el historial de turnos.

  # **Boceto inicial del diseño de clases**

  [boceto final ](https://github.com/user-attachments/assets/cc5f17cd-8ed8-4d30-8448-5e7c9d31ea94)


