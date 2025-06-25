# Principio de Responsabilidad Única (SRP)

### Propósito del Principio:
El principio de responsabilidad única indica que una clase debe tener una sola razón para cambiar, es decir, debe cumplir con una única responsabilidad dentro del sistema.

### Motivación:
En el sistema original, la clase `Turno` gestionaba tanto el almacenamiento de datos como el envío de notificaciones. Esto violaba el SRP, ya que combinaba lógica de negocio con lógica de comunicación.

### Aplicación:
Se creó una clase `Notificacion` independiente que gestiona exclusivamente el envío de mensajes. Así, la clase `Turno` se centra en representar un turno, y `Notificacion` se encarga de comunicar confirmaciones o cancelaciones.

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio SRP:

  ![Diagrama UML](https://github.com/user-attachments/assets/53862668-8ec8-471e-b987-e0d524bf82c0)



