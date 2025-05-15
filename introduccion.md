# Anexo - Introducción al Diseño Orientado a Objetos

## ¿Qué es la Programación Orientada a Objetos?

La Programación Orientada a Objetos (POO) es un paradigma de programación basado en la creación de objetos que representan entidades del mundo real. Cada objeto tiene atributos (características) y métodos (comportamientos). Este enfoque facilita la organización del código, su reutilización y el mantenimiento del software a lo largo del tiempo.

## Los cuatro fundamentos de POO (con ejemplos reales)

### 1. Abstracción
Permite centrarse en los aspectos esenciales de un objeto.  
**Ejemplo**: Un turno médico solo necesita conocer la fecha, la hora, el paciente y el médico asignado, no todos los detalles personales del paciente.

### 2. Encapsulamiento
Protege los datos internos del objeto y solo expone lo necesario.  
**Ejemplo**: La información de contacto de un paciente está protegida; solo personal autorizado puede acceder a ella.

### 3. Herencia
Permite que una clase hija reutilice atributos y métodos de una clase padre.  
**Ejemplo**: `Paciente` y `Médico` pueden heredar de una clase `Persona`.

### 4. Polimorfismo
Distintas clases pueden responder de forma diferente a un mismo mensaje.  
**Ejemplo**: El método `enviarNotificacion()` puede actuar diferente si el canal es correo o SMS.

## Requisitos Funcionales del Sistema

1. Registrar pacientes con nombre, DNI, fecha de nacimiento y contacto.
2. Registrar médicos con nombre, matrícula, especialidad, horario y contacto.
3. Agendar turnos asegurando que no se superpongan.
4. Guardar motivo y observaciones para cada turno.
5. Enviar notificaciones automáticas al confirmar, modificar o cancelar turnos.

## Casos de Uso

### 1. Registrar Paciente
- **Actor**: Recepcionista  
- **Descripción**: Registrar un nuevo paciente.  
- **Flujo principal**:
  1. Ingresar nombre, DNI, fecha de nacimiento y contacto.
  2. Verificar que no esté registrado.
  3. Guardar paciente.
- **Precondición**: Paciente no registrado.  
- **Postcondición**: Paciente registrado en el sistema.

### 2. Registrar Médico
- **Actor**: Administrador  
- **Descripción**: Añadir un nuevo profesional al sistema.  
- **Flujo principal**:
  1. Ingresar nombre, matrícula, especialidad, contacto y horario.
  2. Guardar médico.
- **Precondición**: Médico no registrado.  
- **Postcondición**: Médico disponible para asignación de turnos.

### 3. Asignar Turno
- **Actor**: Recepcionista / Paciente  
- **Descripción**: Reservar turno para una consulta médica.  
- **Flujo principal**:
  1. Seleccionar médico disponible.
  2. Elegir fecha y hora.
  3. Registrar motivo y observaciones.
- **Precondición**: Médico y paciente registrados.  
- **Postcondición**: Turno agendado correctamente.

### 4. Cancelar Turno
- **Actor**: Paciente / Recepcionista  
- **Descripción**: Eliminar turno programado.  
- **Flujo principal**:
  1. Buscar turno.
  2. Confirmar cancelación.
- **Precondición**: Turno confirmado.  
- **Postcondición**: Turno cancelado.

### 5. Enviar Notificación
- **Actor**: Sistema  
- **Descripción**: Informar por correo o SMS una modificación de turno.  
- **Flujo principal**:
  1. Detectar cambio en estado del turno.
  2. Enviar notificación al paciente y al médico.
- **Precondición**: Turno modificado o confirmado.  
- **Postcondición**: Notificación enviada.

## Boceto Inicial del Diseño de Clases

![Diagrama de clases](imagenes/diagrama_clases_inicial.png)

[Ver diseño en línea (Excalidraw)](https://excalidraw.com/#json=agrega-tu-enlace-aquí)

