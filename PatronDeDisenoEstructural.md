# Patrón de Diseño Estructural

## Nombre del patrón: Adapter

## Problema que soluciona
El sistema necesita enviar notificaciones por distintos canales (email, SMS, etc.). Cada proveedor externo tiene una interfaz diferente. Queremos integrar nuevos servicios sin modificar el código existente del sistema.

## Implementación en el proyecto

Se define una interfaz común `INotificador` con el método `enviarNotificacion(turno: Turno): void`.  
Los adaptadores como `AdaptadorEmail` y `AdaptadorSMS` implementan esta interfaz y adaptan el comportamiento de servicios de terceros.

La clase `SistemaTurnos` solo depende de `INotificador`, no importa si internamente se envía un email o un SMS. Así, podemos agregar nuevos canales sin tocar el código del sistema.

## Clases involucradas

- **INotificador**: interfaz con el método `enviarNotificacion(turno: Turno): void`.
- **AdaptadorEmail** / **AdaptadorSMS**: adaptadores concretos que implementan la interfaz y traducen la llamada a servicios externos.
- **ServicioEmailExterno** / **ServicioSMSExterno**: clases simuladas de servicios externos con interfaces distintas.

## Relación con principios SOLID

- **S - Single Responsibility Principle (SRP)**: cada adaptador tiene la única responsabilidad de traducir una interfaz.
- **O - Open/Closed Principle (OCP)**: se pueden agregar nuevos canales de notificación sin modificar el sistema.
- **D - Dependency Inversion Principle (DIP)**: el sistema depende de una abstracción (`INotificador`), no de implementaciones concretas.

## Diagrama UML del patrón


