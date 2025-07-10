# Principio de Responsabilidad Única (SRP)

### Propósito del Principio:
El principio de responsabilidad única indica que una clase debe tener una sola razón para cambiar, es decir, debe cumplir con una única responsabilidad dentro del sistema.

### Problema identificado:
Antes, la clase `Turno` contenía tanto la lógica del turno como la lógica de notificación al paciente. Esto rompe SRP porque mezcla responsabilidades distintas.

### Aplicación:
Creamos dos clases:
- `GestorTurnos`: maneja la lógica de turnos
- `Notificador`: se encarga de enviar notificaciones

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio SRP:

 <img width="590" height="250" alt="srp" src="https://github.com/user-attachments/assets/6869c572-d4aa-4b22-be4e-23465cc72ac4" />





