# Principio de Segregación de Interfaces (ISP)

### Propósito del Principio:
Ninguna clase debe estar obligada a depender de interfaces que no utiliza.

### Motivación:
En el sistema inicial, la clase `Usuario` tenía métodos tanto para médicos como para pacientes, aunque no todos los usuarios necesitaban las mismas funciones.

### Aplicación:
Se segregaron las interfaces en `ITurno` y `IPago`, cada una con los métodos específicos que cada tipo de usuario necesita implementar, evitando dependencias innecesarias.

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio ISP

 ![Diagrama UML](https://github.com/user-attachments/assets/f2ada9b4-7b52-4eec-9ab5-a3c3388348a9)
