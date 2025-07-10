# Principio de Inversión de Dependencias (DIP)

### Propósito del Principio:
Las clases deben depender de abstracciones (interfaces), no de implementaciones concretas.

## Problema identificado

`GestorTurnos` dependía directamente de `RepositorioTurnos`, lo cual hacía difícil cambiar la forma de almacenamiento.

## Ejemplo aplicado

Definimos una interfaz `ITurnoRepository` y `RepositorioTurnosSQL` como implementación.


A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio DIP:


<img width="243" height="374" alt="DIP" src="https://github.com/user-attachments/assets/37705489-4696-4d83-aa27-7a398bd20eeb" />
