# **Principio de Segregación de Interfaces (ISP)**

**Propósito y Tipo del Principio SOLID**

El Principio de Segregación de Interfaces (ISP) es un principio fundamental en el diseño de software que establece que los clientes no deben ser forzados a depender de interfaces que no utilizan. Esto significa que las interfaces deben ser diseñadas de manera que sean específicas y no demasiado generales.

# **Motivación**

El problema que enfrentaba el sistema era que las interfaces eran demasiado generales y forzaban a los clientes a depender de métodos que no utilizaban. Por ejemplo, si una interfaz ITurno tenía métodos para gestionar turnos y también para gestionar pagos, un cliente que solo necesitaba gestionar turnos se vería forzado a depender de la funcionalidad de pagos que no utiliza.

# **Estructura de Clases**

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio ISP

 [Diagrama UML](https://github.com/user-attachments/assets/f2ada9b4-7b52-4eec-9ab5-a3c3388348a9)
