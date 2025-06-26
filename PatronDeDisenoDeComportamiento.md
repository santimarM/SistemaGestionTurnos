# Anexo - Aplicación de Patrón de Diseño de Comportamiento - Observer

## ¿Qué son los patrones de comportamiento?

Los patrones de comportamiento definen cómo **los objetos interactúan entre sí**, promoviendo una comunicación flexible y desacoplada.

---

##  Propósito y Tipo del Patrón

**Patrón:** Observer  
**Tipo:** Comportamiento

**Problema detectado:**  
Se requiere que diferentes componentes del sistema sean notificados automáticamente cuando se cancela o confirma un turno, sin acoplarlos entre sí.

**Solución:**  
El patrón Observer permite que objetos como `Paciente`, `Médico` y `Recepcionista` se **suscriban a eventos** del sistema de turnos y reciban actualizaciones en tiempo real.

---

##  Motivación

Actualmente, si un turno es cancelado, no hay una forma automatizada de avisar a todos los implicados. Con Observer:

- `Turno` actúa como "Sujeto" (Subject).
- `Paciente` y `Médico` actúan como "Observadores" (Observers).
- Se notifica automáticamente cuando hay cambios.

---

##  Estructura de Clases (Diagrama UML)
![PatronDeDisenoDeComportamiento md drawio](https://github.com/user-attachments/assets/c1bdf15b-b455-44a5-b7ca-4ae3b64a66db)



