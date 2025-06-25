# Principio de Abierto/Cerrado (OCP)

### Propósito del Principio:
Una entidad de software (clase, módulo, función) debe estar abierta para la extensión, pero cerrada para la modificación.

### Motivación:
En versiones iniciales, para agregar un nuevo tipo de notificación (por ejemplo, WhatsApp además de email y SMS), era necesario modificar la clase `Notificacion`.

### Aplicación:
Se definió una interfaz `INotificador` y se crearon implementaciones concretas (`EmailNotificador`, `SMSNotificador`, `WhatsAppNotificador`). Así, el sistema puede extenderse agregando nuevas clases sin modificar las existentes.

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio OCP:

 ![Diagrama UML](https://github.com/user-attachments/assets/f00b6cae-3929-41f2-94b8-2107da6edaeb)

