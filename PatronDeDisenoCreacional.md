# Patrón de Diseño Creacional

## Nombre del patrón: Factory Method

## Problema que soluciona
Permite instanciar distintos tipos de turnos (presenciales y virtuales) sin que el sistema esté acoplado a las clases concretas. Esto facilita la escalabilidad del sistema para agregar nuevos tipos de turnos sin modificar código existente.

## Implementación en el proyecto

Se crea una interfaz `TurnoFactory` con el método `crearTurno(...)`. Las fábricas concretas como `TurnoPresencialFactory` y `TurnoVirtualFactory` implementan este método, devolviendo instancias de `TurnoPresencial` y `TurnoVirtual`, respectivamente.

La clase `SistemaTurnos` usa una fábrica concreta, pero solo conoce la interfaz `TurnoFactory`, lo que desacopla la lógica de creación del tipo de turno.

## Clases involucradas

- **TurnoFactory** (interfaz): define el método `crearTurno(...)`.
- **TurnoPresencialFactory** / **TurnoVirtualFactory**: implementan la interfaz y crean sus tipos de turno.
- **Turno** (abstracta o clase base).
- **TurnoPresencial** / **TurnoVirtual**: heredan de `Turno`.

## Relación con principios SOLID

- **S - Single Responsibility Principle (SRP)**: cada clase tiene una única responsabilidad (crear un tipo específico de turno).
- **O - Open/Closed Principle (OCP)**: se pueden agregar nuevos tipos de turnos sin modificar las clases existentes.
- **D - Dependency Inversion Principle (DIP)**: el sistema depende de la abstracción `TurnoFactory`, no de implementaciones concretas.

## Diagrama UML del patrón

<img width="1024" height="1024" alt="factori" src="https://github.com/user-attachments/assets/ae1b4251-ed4c-462c-9626-65784dd90734" />


