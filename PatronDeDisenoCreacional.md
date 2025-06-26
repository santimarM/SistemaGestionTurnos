# Anexo - Aplicación de Patrón de Diseño Creacional - Singleton

## ¿Qué son los patrones creacionales?

Los patrones de diseño creacionales se encargan de la **creación de objetos**. Permiten encapsular la lógica de instancia, evitando la creación directa y facilitando el control del ciclo de vida.

---

## Propósito y Tipo del Patrón

**Patrón:** Singleton  
**Tipo:** Creacional

**Problema detectado:**  
En un sistema de turnos médicos, es necesario asegurar que haya **una única instancia central de agenda** que controle los turnos disponibles, evitando inconsistencias o duplicación de datos si se accede desde múltiples lugares.

**Solución:**  
El patrón Singleton asegura que solo haya una instancia de la clase `AgendaTurnos`, accesible globalmente y sincronizada para todos los usuarios.

---

## Motivación

La agenda de turnos debe ser única y centralizada para que todos los módulos (paciente, médico, recepcionista) accedan y modifiquen el mismo objeto. La creación de múltiples instancias llevaría a errores graves (como turnos duplicados o inconsistentes). Singleton permite:

- Centralizar el acceso.
- Evitar múltiples instancias.
- Asegurar integridad de la información.

---

## Estructura de Clases (Diagrama UML)
![diseñocreacional drawio](https://github.com/user-attachments/assets/9b2fb9c8-b0cd-4ca0-aeb2-fda3b5c913a5)

