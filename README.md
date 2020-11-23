
**Proyecto Final:** 

**Equipo:** Delfines en Éxtasis

**Integrantes:**
- Jacqueline Lira Chávez - 
- José Luis Sandín Espinosa -
- Mónica Hernández Martínez - 163543
- Piero ...

# Índice

1. [Requrimientos del Sistema](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#1-requerimientos-del-sistema)
    1. [Introducción](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#introducción)
    2. [Descripción general](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#descripción-general)
    3. [Requerimientos de interfaz externa](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#requerimientos-de-interfaz-externa)
    4. [Funcionalidades del sistema](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#funcionalidades-del-sistema)
    5. [Otros requerimientos no funcionales](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#otros-requerimientos-no-funcionales)
2. [Plan de Calidad](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#2-plan-de-calidad)
    1. [Identificador del plan de prueba](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#identificador-del-plan-de-prueba)
    2. [Referencias](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#referencias)
    3. [Introducción](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#introducción-1)
    4. [Elementos de prueba](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#elementos-de-prueba)
    5. [Problemas de riesgo del software](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#problemas-de-riesgo-del-software)
    6. [Funcionalidades a probar](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#funcionalidades-a-probar)
    7. [Funcionalidades que no deben probarse](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#funcionalidades-que-no-deben-probarse)
    8. [Enfoque](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#enfoque)
    9. [Críterios de aprobación/falla](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#críterios-de-aprobación/falla)
    10. [Criterios de suspensión y requisitos de reanudación](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#críterios-de-suspensión-y-requisitos-de-reanudación)
    11. [Entregables de prueba](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#entregables-de-prueba)
    12. [Tareas de pruebas restantes](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#tareas-de-pruebas-restantes)
    13. [Necesidades ambientales](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#necesidades-ambientales)
    14. [Necesidades del personal y capacitación](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#necesidades-del-personal-y-capacitación)
    15. [Responsabilidades](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#responsabilidades)
    16. [Calendario](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#calendario)
    17. [Planificación de riesgos y contingencias](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#planificación-de-riesgos-y-contingencias)
    18. [Aprobación](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#aprobación)
    19. [Glosario](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#glosario)
3. [Arquitectura](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#3-arquitectura)
4. [Metodología](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#4-metodología)
5. [Instrucciones para replicar](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#5-instrucciones-para-replicar)
6. [Presentación](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#6-presentación)

# 1. Requerimientos del Sistema

## Introducción

### Propósito
En este documento se describen las especificaciones de los requerimientos del sistema _NombreApp_, el cual es un gestor de chats exclusivo para el Instituto Tecnológico Autónomo de México (ITAM).  _NombreApp_ es un medio para que los alumnos del ITAM puedan comunicarse entre ellos, así como también poder entablar conversaciones con profesores y del personal administrativo. _NombreApp_ tiene como objetivo mejorar la experiencia de los estudiantes facilitándoles los recursos para poder expresarse y desarrollarse de la mejor manera en su vida diaria como estudiante. A continuación, proporcionaremos a describir detalladamente el software de _NombreApp_ 1.0.

### Convenciones del documento

En este documento se hace uso del estándar de la IEEE para SRS del SIO/IEC/IEEE 29148.

Para el manejo de las prioridades en las funcionalidades se manejará el rango 1-3, donde 1 significa que la prioridad es indispensable y 3 es que se puede prescindir de ella.

### Público objetivo y sugerencicas de lectura

Este documento está intencionado para los desarrolladores que estan acargo del mantenimiento del sistema _NombreApp_, se espera que este cuerpo sea parte del personal administritativo de cómputo del ITAM. Se les sugiere leer todo el documento la primera vez, y posteriormente apoyarse en el índice para poder tener un lectura rápida de las dudas que se generen en un futuro sobre el sistema.

### Alcance del producto



## Descripción general

### Perspectiva del producto

### Funciones del producto

### Clases y características del usuario

### Entorno operativo

### Restricciones de diseño e implementación

### Documentación del usuario

### Suposiciones y dependencias

## Requerimientos de interfaz externa

### Interfaces de usuario

### Interfaces de hardware

### Interfaces de software

### Interfaces de comunicaciones

## Funcionalidades del sistema

### Iniciar sesión

### Buscar contacto

### Creación de chat grupales

### 

## Otros requerimientos no funcionales

### Requerimientos de rendimiento

### Requerimientos de seguridad (Safety)

### Requerimientos de seguridad (Security)

### Atributos de calidad de software

### Reglas de negocio


# 2. Plan de Calidad

## Identificador del plan de prueba

## Referencias

## Introducción

## Elementos de prueba

## Problemas de riesgo del software

## Funcionalidades a probar

## Funcionalidades que no deben probarse

## Enfoque

## Críterios de aprobación/falla

## Criterios de suspensión y requisitos de reanudación

## Entregables de prueba

## Tareas de pruebas restantes

## Necesidades ambientales

## Necesidades del personal y capacitación

## Responsabilidades

## Calendario

## Planificación de riesgos y contingencias

## Aprobación

## Glosario

# 3. Arquitectura

# 4. Metodología

# 5. Instrucciones para replicar

# 6. Presentación

Podrá encontrar la presentación del proyecto final [aquí]()




