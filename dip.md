# Principio de Inversión de Dependencias (DIP)

### Propósito del Principio:
Las clases deben depender de abstracciones (interfaces), no de implementaciones concretas.

### Motivación:
La clase `Sistema` creaba instancias concretas de `EmailNotificador`, lo que dificultaba el cambio de canal de notificación.

### Aplicación:
Se inyecta una instancia de `INotificador` al sistema mediante el constructor o un patrón como fábrica o inyección de dependencias. Esto permite desacoplar la lógica del sistema de la implementación concreta de notificaciones.


A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio DIP:

 ![Diagrama UML](https://github.com/user-attachments/assets/7b493c19-eb59-4d65-8444-4bf0a67f5d89)
