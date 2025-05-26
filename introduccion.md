# Anexo - Introducción al Diseño Orientado a Objetos

## ¿Qué es la Programación Orientada a Objetos (POO)?

La POO es un paradigma de programación que organiza el software en objetos, los cuales combinan datos (atributos) y comportamientos (métodos). Este enfoque permite modelar el mundo real de manera más natural, facilitando el mantenimiento y la reutilización del código.

## Importancia

- Promueve el diseño modular.
- Favorece la reutilización mediante la herencia.
- Facilita el mantenimiento y la escalabilidad.
- Permite representar sistemas complejos de forma clara y estructurada.

---

## Los Cuatro Fundamentos de la POO

### 1. **Abstracción**
Permite representar objetos del mundo real destacando solo los detalles relevantes.

_Ejemplo:_ Un paciente es representado por su nombre, DNI y contacto, sin necesidad de incluir otros aspectos como su dirección postal o estado civil.

### 2. **Encapsulamiento**
Oculta la implementación interna de un objeto, exponiendo solo lo necesario mediante métodos públicos.

_Ejemplo:_ El historial de turnos de un paciente no puede modificarse directamente, sino mediante métodos específicos.

### 3. **Herencia**
Permite que una clase herede atributos y métodos de otra, promoviendo la reutilización.

_Ejemplo:_ `Usuario` puede ser una clase genérica, y `Paciente` y `Médico` heredan de ella.

### 4. **Polimorfismo**
Permite que un mismo método se comporte de distintas formas según el objeto que lo invoque.

_Ejemplo:_ Un método `mostrarPerfil()` puede tener un comportamiento diferente si lo ejecuta un paciente o un médico.

---

## Requisitos Funcionales Iniciales del Sistema

1. Registrar pacientes y profesionales de la salud.
2. Asignar turnos según disponibilidad.
3. Enviar notificaciones por cambios en los turnos.
4. Evitar superposición de turnos por médico.
5. Consultar historial de turnos de cada paciente.

---

## Casos de Uso

### Caso de Uso 1: Registrar Paciente

- **Actor:** Recepcionista
- **Descripción breve:** Permite dar de alta a un nuevo paciente.
- **Flujo principal:** El recepcionista ingresa los datos, el sistema valida y guarda.
- **Precondición:** El paciente no debe estar registrado.
- **Postcondición:** El paciente queda registrado en el sistema.

### Caso de Uso 2: Asignar Turno

- **Actor:** Paciente / Recepcionista
- **Descripción breve:** Se asigna un turno con un profesional.
- **Flujo principal:** Se selecciona médico, fecha y hora, el sistema verifica disponibilidad y guarda.
- **Precondición:** El paciente debe estar registrado.
- **Postcondición:** Turno registrado y confirmado.

### Caso de Uso 3: Cancelar Turno

- **Actor:** Paciente / Médico / Recepcionista
- **Descripción breve:** Permite cancelar un turno ya asignado.
- **Flujo principal:** Se selecciona el turno y se cambia el estado a "Cancelado".
- **Precondición:** Turno debe existir.
- **Postcondición:** Turno queda cancelado.

### Caso de Uso 4: Consultar Historial Médico

- **Actor:** Médico
- **Descripción breve:** Accede al historial de turnos de un paciente.
- **Flujo principal:** Se selecciona el paciente y se muestra su historial.
- **Precondición:** Médico autenticado y paciente registrado.
- **Postcondición:** Historial visualizado.

### Caso de Uso 5: Notificar Cambios

- **Actor:** Sistema
- **Descripción breve:** Envía notificación automática por cambios en turnos.
- **Flujo principal:** Ante cambio de estado, se envía email/SMS.
- **Precondición:** Cambio en turno confirmado.
- **Postcondición:** Notificación enviada.

---

## Boceto Inicial del Diseño de Clases

