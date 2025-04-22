# **Principio de Sustitución de Liskov (LSP)**

**Propósito y Tipo del Principio SOLID**

El Principio de Sustitución de Liskov (LSP) es un principio fundamental en el diseño de software que establece que los objetos de un tipo deben ser reemplazables por objetos de sus subtipos sin afectar la corrección del programa. Esto significa que una clase derivada debe comportarse de manera consistente con su clase base.

**Motivación**

El problema que enfrentaba el sistema era que las clases derivadas no se comportaban de manera consistente con sus clases base, lo que provocaba errores y comportamientos inesperados. Por ejemplo, si una clase Ave tenía un método volar() y una clase Pinguino heredaba de Ave, pero no podía volar, esto podría provocar problemas si se utilizaba un objeto Pinguino en un contexto donde se esperaba un objeto Ave que pudiera volar.

**Estructura de Clases**

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio LSP:

 [Diagrama UML](https://github.com/user-attachments/assets/cc9fe5f1-e4eb-48cf-ba1d-4b01633f6bae)

