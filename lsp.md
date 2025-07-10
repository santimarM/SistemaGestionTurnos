# Principio de Sustitución de Liskov (LSP)

### Propósito del Principio:
Los objetos de una subclase deben poder sustituir a objetos de su superclase sin alterar el comportamiento esperado del sistema.

## Problema identificado

Antes usábamos ejemplos fuera del contexto del sistema (como el pingüino). No había una jerarquía coherente en el diseño.

## Ejemplo aplicado

Definimos una clase base `Usuario` con subclases `Paciente` y `Medico`, que pueden sustituirse sin romper el sistema.

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio LSP:

<img width="509" height="234" alt="lsp" src="https://github.com/user-attachments/assets/9cf6da8c-6ad2-4a66-809f-56235edd8286" />


