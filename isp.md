# Principio de Segregación de Interfaces (ISP)

### Propósito del Principio:
Ninguna clase debe estar obligada a depender de interfaces que no utiliza.

## Problema identificado

Una interfaz general `IUsuario` tenía métodos que no aplicaban a todos los usuarios (ej. `verHistorial()` para un paciente).

## Ejemplo aplicado

Se dividen las interfaces según roles específicos.

A continuación, se muestra un diagrama UML que ilustra cómo las clases principales del proyecto se relacionan entre sí al aplicar el principio SRP:

<img width="509" height="201" alt="isp" src="https://github.com/user-attachments/assets/54f196ff-efe3-400d-b41a-b9fb35a336f7" />
