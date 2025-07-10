# Principio de Abierto/Cerrado (OCP)

### Propósito del Principio:
Una entidad de software (clase, módulo, función) debe estar abierta para la extensión, pero cerrada para la modificación.

## Problema identificado

La clase `Notificador` tenía métodos fijos para email. Para agregar WhatsApp o SMS, debíamos modificarla.

## Ejemplo aplicado

Creamos una interfaz `INotificador` y varias implementaciones (`EmailNotificador`, `WhatsAppNotificador`).

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio OCP:

 <img width="759" height="342" alt="ocp" src="https://github.com/user-attachments/assets/11b3cd87-d17b-4608-9968-bb820770a5e8" />


