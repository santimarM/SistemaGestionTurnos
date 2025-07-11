# Patrón de Diseño de Comportamiento

## Nombre del patrón: Observer

## Problema que soluciona
El sistema necesita notificar automáticamente a distintos observadores (como pacientes o médicos) cuando se genera o actualiza un turno, sin acoplar fuertemente estas clases entre sí. Se busca mantener una arquitectura flexible y extensible.

## Implementación en el proyecto

Se define una interfaz `Observador` con el método `actualizar(turno: Turno): void`.  
La clase `Turno` actúa como **Sujeto (Subject)** y mantiene una lista de observadores (como `Paciente` y `Medico`).  
Cuando se modifica el turno, el sistema llama a `notificar()` para que todos los observadores registrados reaccionen en consecuencia.

## Clases involucradas

- **Turno (Sujeto)**: contiene métodos `agregarObservador()`, `eliminarObservador()`, y `notificar()`.
- **Observador (Interfaz)**: define el método `actualizar(turno: Turno)`.
- **Paciente** y **Medico**: implementan `Observador` y definen cómo reaccionar cuando se actualiza un turno.

## Relación con principios SOLID

- **O - Open/Closed Principle**: se pueden agregar nuevos observadores sin modificar el sujeto.
- **L - Liskov Substitution Principle**: cualquier clase que implemente `Observador` puede reemplazar otra.
- **D - Dependency Inversion Principle**: el sujeto depende de una abstracción (`Observador`), no de clases concretas.

## Diagrama UML del patrón

<img width="1024" height="1024" alt="ultimo }" src="https://github.com/user-attachments/assets/be2b6fb8-13cb-48e5-9722-8c56390f2c5e" />


