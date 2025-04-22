# **Principio de Abierto/Cerrado (OCP)**

**Propósito y Tipo del Principio SOLID**

El Principio de Abierto/Cerrado (OCP) es un principio fundamental en el diseño de software que establece que una clase debe estar abierta para la extensión pero cerrada para la modificación. Esto significa que una clase debe permitir agregar nuevas funcionalidades sin modificar su código existente.

**Motivación**

El problema que enfrentaba el sistema era que las clases estaban diseñadas de manera que cualquier cambio en la funcionalidad requería modificar el código existente. Esto hacía que el sistema fuera rígido y difícil de mantener. Por ejemplo, si una clase se encargaba de gestionar los turnos de los médicos, cualquier cambio en la lógica de gestión de turnos requeriría modificar la clase existente.

**Estructura de Clases**

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio OCP:

 [Diagrama UML](https://github.com/user-attachments/assets/f00b6cae-3929-41f2-94b8-2107da6edaeb)
