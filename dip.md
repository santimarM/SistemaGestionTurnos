# **Principio de Inversión de Dependencias (DIP)**

**Propósito y Tipo del Principio SOLID**

El Principio de Inversión de Dependencias (DIP) es un principio fundamental en el diseño de software que establece que las clases de alto nivel no deben depender de clases de bajo nivel, sino que ambas deben depender de abstracciones. Esto significa que las dependencias deben ser invertidas, de manera que las clases de alto nivel dependan de interfaces o abstracciones en lugar de clases concretas.

# **Motivación**

El problema que enfrentaba el sistema era que las clases de alto nivel dependían directamente de clases de bajo nivel, lo que hacía que el sistema fuera rígido y difícil de mantener. Por ejemplo, si una clase Recepcionista dependía directamente de una clase Turno, cualquier cambio en la clase Turno podría afectar la clase Recepcionista.


# **Estructura de Clases**

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio DIP:

 [Diagrama UML](https://github.com/user-attachments/assets/7b493c19-eb59-4d65-8444-4bf0a67f5d89)
