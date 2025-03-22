 Introducción


 Descripción del paradigma orientado a objetos
La programación orientada a objetos (POO) es un paradigma de programación que se basa en la idea de que los programas deben estar organizados en torno a objetos y clases, en lugar de funciones y procedimientos. La POO es importante porque permite la creación de programas más modulares, reutilizables y fáciles de mantener.


 Los cuatro fundamentos de POO
- Encapsulación: La encapsulación es el proceso de ocultar los detalles de implementación de un objeto y solo exponer sus características y comportamientos esenciales. Por ejemplo, un automóvil puede ser visto como un objeto que encapsula su motor, transmisión y otros componentes.
- Herencia: La herencia es el mecanismo por el cual una clase puede heredar las características y comportamientos de otra clase. Por ejemplo, un camión puede ser visto como una clase que hereda las características de un automóvil.
- Polimorfismo: El polimorfismo es la capacidad de un objeto para tomar diferentes formas dependiendo del contexto en el que se utilice. Por ejemplo, un objeto que representa un animal puede ser visto como un perro, gato o caballo dependiendo de cómo se utilice.
- Abstracción: La abstracción es el proceso de representar conceptos y objetos complejos de manera simple y esencial. Por ejemplo, un mapa puede ser visto como una abstracción de un territorio.


 Requisitos iniciales del sistema
- El sistema debe permitir la creación de turnos para diferentes servicios.
- El sistema debe permitir la asignación de turnos a diferentes empleados.
- El sistema debe permitir la visualización de la agenda de turnos para cada empleado.
- El sistema debe permitir la edición y eliminación de turnos.
- El sistema debe permitir la generación de informes sobre la utilización de los servicios.

Caso de uso 1: Crear turno
- Nombre del caso de uso: Crear turno
- Actores involucrados: Empleado, Sistema
- Descripción breve: El empleado crea un nuevo turno para un servicio.
- Flujo de eventos:
1. El empleado ingresa al sistema.
2. El empleado selecciona el servicio para el cual desea crear el turno.
3. El empleado ingresa la fecha y hora del turno.
4. El sistema verifica la disponibilidad del servicio en la fecha y hora seleccionadas.
5. El sistema crea el turno y lo asigna al empleado.
- Precondiciones: El empleado debe estar registrado en el sistema y tener permisos para crear turnos.
- Postcondiciones: El turno se crea y se asigna al empleado.


Caso de uso 2: Asignar turno a empleado
- Nombre del caso de uso: Asignar turno a empleado
- Actores involucrados: Administrador, Empleado, Sistema
- Descripción breve: El administrador asigna un turno a un empleado.
- Flujo de eventos:
1. El administrador ingresa al sistema.
2. El administrador selecciona el turno que desea asignar.
3. El administrador selecciona al empleado al que desea asignar el turno.
4. El sistema verifica que el empleado esté disponible en la fecha y hora del turno.
5. El sistema asigna el turno al empleado.
- Precondiciones: El administrador debe estar registrado en el sistema y tener permisos para asignar turnos.
- Postcondiciones: El turno se asigna al empleado.


Caso de uso 3: Visualizar agenda de turnos
- Nombre del caso de uso: Visualizar agenda de turnos
- Actores involucrados: Empleado, Sistema
- Descripción breve: El empleado visualiza su agenda de turnos.
- Flujo de eventos:
1. El empleado ingresa al sistema.
2. El empleado selecciona la opción para visualizar su agenda de turnos.
3. El sistema muestra la agenda de turnos del empleado.
- Precondiciones: El empleado debe estar registrado en el sistema.
- Postcondiciones: El empleado visualiza su agenda de turnos.


 Caso de uso 4: Cancelar turno
- Nombre del caso de uso: Cancelar turno
- Actores involucrados: Empleado, Sistema
- Descripción breve: El empleado cancela un turno.
- Flujo de eventos:
1. El empleado ingresa al sistema.
2. El empleado selecciona el turno que desea cancelar.
3. El sistema verifica que el empleado tenga permisos para cancelar el turno.
4. El sistema cancela el turno y notifica al cliente.
- Precondiciones: El empleado debe estar registrado en el sistema y tener permisos para cancelar turnos.
- Postcondiciones: El turno se cancela y se notifica al cliente.


Caso de uso 5: Generar informe de turnos
- Nombre del caso de uso: Generar informe de turnos
- Actores involucrados: Administrador, Sistema
- Descripción breve: El administrador genera un informe de turnos.
- Flujo de eventos:
1. El administrador ingresa al sistema.
2. El administrador selecciona la opción para generar un informe de turnos.
3. El sistema muestra las opciones para filtrar el informe (fecha, empleado, servicio, etc.).
4. El administrador selecciona las opciones de filtrado y el sistema genera el informe.
- Precondiciones: El administrador debe estar registrado en el sistema y tener permisos para generar informes.
- Postcondiciones: El informe de turnos se genera y se muestra al administrador.
