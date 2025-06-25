# Principio de Sustitución de Liskov (LSP)

### Propósito del Principio:
Los objetos de una subclase deben poder sustituir a objetos de su superclase sin alterar el comportamiento esperado del sistema.

### Motivación:
Si `Medico` y `Paciente` heredan de una clase `Usuario`, cualquier operación que funcione con `Usuario` debería funcionar correctamente con instancias de `Medico` o `Paciente`.

### Aplicación:
Se aseguraron los métodos comunes (`getNombre`, `getContacto`) en la superclase `Usuario`, evitando que las subclases necesiten redefinir comportamientos que rompan la funcionalidad general.

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio LSP:

 [Diagrama UML](https://github.com/user-attachments/assets/cc9fe5f1-e4eb-48cf-ba1d-4b01633f6bae)

