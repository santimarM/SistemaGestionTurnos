# Anexo - Principios SOLID

Los principios SOLID son una guía fundamental para diseñar software orientado a objetos que sea mantenible, escalable y fácil de entender. En este proyecto, se aplican estos principios al diseño del sistema de gestión de turnos médicos para asegurar una estructura coherente y flexible frente a cambios futuros.

## ¿Qué son los principios SOLID?

El acrónimo SOLID representa cinco principios clave en la programación orientada a objetos:

1. **SRP - Principio de Responsabilidad Única (Single Responsibility Principle)**  
   Una clase debe tener una única razón para cambiar. Cada clase debe encargarse de una sola responsabilidad dentro del sistema.

2. **OCP - Principio Abierto/Cerrado (Open/Closed Principle)**  
   El software debe estar abierto a la extensión, pero cerrado a la modificación. Es decir, podemos agregar nuevas funcionalidades sin alterar las existentes.

3. **LSP - Principio de Sustitución de Liskov (Liskov Substitution Principle)**  
   Las clases derivadas deben poder sustituir a sus clases base sin alterar el funcionamiento del programa.

4. **ISP - Principio de Segregación de Interfaces (Interface Segregation Principle)**  
   Una clase no debe verse obligada a implementar interfaces que no utiliza. Es mejor tener varias interfaces específicas que una genérica y pesada.

5. **DIP - Principio de Inversión de Dependencias (Dependency Inversion Principle)**  
   Los módulos de alto nivel no deben depender de módulos de bajo nivel. Ambos deben depender de abstracciones.

---

## Aplicación en este proyecto

En este sistema, los principios SOLID se reflejan de la siguiente manera:

- Se separan claramente las responsabilidades entre clases como `Turno`, `Paciente`, `Médico`, `Notificador` y `Administrador`.
- Se busca que las clases puedan ampliarse sin modificarse directamente (por ejemplo, agregar nuevos tipos de notificación sin alterar el flujo principal).
- Se aplican herencias responsables, permitiendo la sustitución sin romper la lógica del sistema.
- Se definen interfaces concretas y específicas donde sea necesario.
- Se promueve el uso de dependencias basadas en abstracciones para facilitar pruebas y cambios futuros.

Para cada principio, se ha elaborado un archivo específico que explica su aplicación, justificación y se acompaña de un diagrama UML correspondiente:

- [Principio SRP - Responsabilidad Única](srp.md)
- [Principio OCP - Abierto/Cerrado](ocp.md)
- [Principio LSP - Sustitución de Liskov](lsp.md)
- [Principio ISP - Segregación de Interfaces](isp.md)
- [Principio DIP - Inversión de Dependencias](dip.md)

