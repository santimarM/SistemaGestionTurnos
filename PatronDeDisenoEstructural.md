# Anexo - Aplicación de Patrón de Diseño Estructural - Adapter

## ¿Qué son los patrones estructurales?

Los patrones estructurales se centran en **la forma en que las clases y objetos se organizan**, permitiendo la colaboración entre interfaces incompatibles.

---

## Propósito y Tipo del Patrón

**Patrón:** Adapter  
**Tipo:** Estructural

**Problema detectado:**  
El sistema necesita conectarse a distintos formatos de historial médico externos, pero las interfaces no son compatibles con el modelo interno.

**Solución:**  
El Adapter actúa como un **puente entre el historial externo y la estructura interna**, traduce las llamadas y permite que el sistema procese los datos correctamente.

---

## Motivación

Hay diferentes proveedores de sistemas de salud que almacenan los historiales en formatos diversos. No es posible modificar cada uno, pero sí implementar un `AdapterHistorialExterno` que traduzca estos datos al formato esperado por `Paciente`.

---

## Estructura de Clases (Diagrama UML)

![PatronDeDisenoEstructural md drawio](https://github.com/user-attachments/assets/7d2d36a8-bc12-489b-94e5-5e718c6c986f)

