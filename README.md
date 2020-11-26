![](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/encabezado.png)

![](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/logo.png)

**Proyecto Final: ConectaITAM** 

**Equipo:** Delfines en Éxtasis

**Integrantes:**
- Jacqueline Lira Chávez - 167334
- José Luis Sandín Espinosa - 179706
- Mónica Hernández Martínez - 163543
- Piero Vera Stephens - 179915

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

En este documento se describen las especificaciones de los requerimientos del sistema ConectaITAM, el cual es un gestor de chats exclusivo para el Instituto Tecnológico Autónomo de México (ITAM).  ConectaITAM es un medio para que los alumnos del ITAM puedan comunicarse entre ellos, así como también poder entablar conversaciones con profesores y del personal administrativo. ConectaITAM tiene como objetivo mejorar la experiencia de los estudiantes facilitándoles los recursos para poder expresarse y desarrollarse de la mejor manera en su vida diaria como estudiante. A continuación, proporcionaremos a describir detalladamente el software de ConectaITAM 1.0.

### Convenciones del documento

En este documento se hace uso del estándar de la IEEE para SRS del SIO/IEC/IEEE 29148.

Para el manejo de las prioridades en las funcionalidades se manejará el rango 1-3, donde 1 significa que la prioridad es indispensable y 3 es que se puede prescindir de ella.

### Público objetivo y sugerencicas de lectura

Este documento está intencionado para los desarrolladores que estan acargo del mantenimiento del sistema ConectaITAM, se espera que este cuerpo sea parte del personal administritativo de cómputo del ITAM. Se les sugiere leer todo el documento la primera vez, y posteriormente apoyarse en el índice para poder tener un lectura rápida de las dudas que se generen en un futuro sobre el sistema.

### Alcance del producto

ConectaITAM es un software que permitirá a los alumnos del ITAM tener una aplicación para la comunicación rápida con todos los estudiantes, profesores y personal administrativo del ITAM.

ConectaITAM tiene como metas:
- Proporcionar un nuevo medio para la comunicación entre toda la comunidad. Ir más allá del correo electrónico institucional.
- Llegar a ser el principal conducto de comunicación para los asuntos escolares dentro de la comunidad.
- Mejorar las relaciones alumno-profesor, alumno-personal administrativo y profesor-personal administrativo.
- Mejorar la experiencia de vida institucional.
    + Los alumnos tendrán un medio para obtener de manera fácil información sobre las dudas que pueda tener tanto de la clase como de los asuntos administrativos.
    + Los profesores tendrán un medio para poder dar a conocer notificiones urgentes como avisos imprevistos, así como también podrán ofrecer de manera personalizada ayuda a sus clases y alumnos.
    + Los administrativos podrán reducir su carga de trabajo pues a través de la aplicación del chat podrán ofrecer información general, por medio de un chatbot, y evitar que los alumnos acudan a sus instalaciones para tareas pequeñas y monótonas.

## Descripción general

### Perspectiva del producto

ConectaITAM es un sistema que será añadido al conjunto de aplicaciones ofrecidas por el ITAM, así como también busca complementar a las ya existentes, tal como comunidad ITAM y Servicios Web.

A continuación, se muestra un diagrama que ilustra las entidades externas y los actores del sistema.

![](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/mapa1.png)

### Funciones del producto

El sistema ConectaITAM proveerá de las siguientes funcionalidades principales:

+ **PF-1:** Almacenar, desplegar y actualizar los chats de cada usuario del sistema.
+ **PF-2:** Buscar usuarios a través del nombre, correo institucional o por clases inscritas relacionadas.
+ **PF-3:** Capacidad de enviar mensajes directos y archivos multimedia através de los chats de sus contactos o de usuarios buscados.
+ **PF-4:** Creación y gestión tanto de chats grupales privados como predefinidos.
+ **PF-5:** Creación y gestión de las conversaciones mostradas en la bandeja de entrada del usuario.
+ **PF-6:** Capacidad para entablar conversación con el chatbot de ayuda de servicios escolares administrativos.
+ **PF-7:** Capacidad para entablar conversación con una persona de servicios escolares en el caso de ser necesario. 

### Clases y características del usuario

Los usuarios a interactuar con ConectaITAM son:

+ **Administradores:** Grupo encargado de administrar y mantener la aplicación ConectaITAM, tanto de la base de datos como de los sistemas relacionados a este. Se espera en un inicio gran interación con la aplicación pues son los encargados de la creación de los chats grupales predefinidos, relacionados a las clases inscritas del alumno, y de la gestión del chatbot. De los administradores se espera un alto conocimiento del software.
+ **Estudiantes:** Será el usuario que tendrá mayor contacto con la aplicación, se espera un uso diario. Se considera estudiante a todo aquel que curse alguna clase en el ITAM, sea licenciatura, ingeniería o algún posgrado. Se esperan las siguientes interacciones: envíar y recibir mensajes, crear y gestionar chats grupales, buscar usuarios.
+ **Personal administrativo:** Se espera un menor contacto del personal administrativo, pues el objetivo es disminuir su trabajo con el chatbot. Se considera personal administrativo a todas aquellas personas que pertenecen a Servicios Escolares y a administrativos de los departamentos acádemicos. Se esperan las siguientes interacciones: dar información tanto general como personal a los alumnos, brindar apoyo y resolver dudas sobre su vida académica; envíar y recibir mensajes de otros usuarios en el caso necesario. 
+ **Profesores:** Será el segundo usuario con mayor contacto con la aplicación. Se concidera profesor a todos los catedráticos que se encuentren impartiendo alguna clase en la institución. Se esperan las siguientes interacciones: envíar y recibir mensajes con otros usuarios, buscar usuarios.

### Entorno operativo

ConectaITAM está desarrollado para poder convivir con el siguiente entorno: 
+ **OE-1:** No hay restricción geográfica de dónde operará la aplicación.
+ **OE-2:** Deberá operar en los navegadores web principales: Chrome, Firefox, Safari y Opera.
+ **OE-3:** Se deberá proporcionar un servicio continuo y estable.

### Restricciones de diseño e implementación

ConectaITAM estará restringido a las siguientes limitaciones:
+ **DIC-1:** Se deberá cumplir con las políticas de información, seguridad y privacidad del ITAM.
+ **DIC-2:** Se deberá usar las tecnologías de acuerdo a los estándares del ITAM.
+ **DIC-3:** Se limitará el tamaño de los archivos multimedia compartidos mediante el chat.
+ **DIC-4:** Se limitará el tipo de archivos multimedia compartidos mediante el chat. Solo ciertas extenciones serán válidas.
+ **DIC-5:** No se permitirán llamadas ni videollamadas.

### Documentación del usuario

ConectaITAM proveerá dos tipos de apoyo para sus usuarios.
+ Dentro de la aplicación existirá un botón de ayuda, el cual incluirá un tutorial interáctivo para los usuarios.
+ Fuera de la aplicación el ITAM proveerá un manual de usuario en su portal principal.
    - Este manual de usuario será envíado también a través del correo institucional cuando la aplicación esté en uso.

### Suposiciones y dependencias

ConectaITAM contará con las siguientes dependencias:
+ **AS-1:** Las cuentas de usuarios de la aplicación están ligadas a la autentificación del ITAM. Ninguna persona que no posea un correo institucional verificado podrá tener acceso a la aplicación.
+ **AS-2:** Se queda sujeto al funcionamiento de los servidores y de la base de datos del ITAM.
+ **AS-3:** Se asume que la aplicación podrá funcionar adecuadamente con aproximadamente 6,000 usuarios.
+ **AS-4:** Se presume que los usuarios tendrán actualizado sus sistemas operativos y navegadores web.

## Requerimientos de interfaz externa - ¡¡FALTA!!

### Interfaces de usuario

### Interfaces de hardware

### Interfaces de software

### Interfaces de comunicaciones

## Funcionalidades del sistema - ¡¡FALTA!!

### Iniciar sesión 

### Buscar contacto

### Creación de chat grupales

### ...

## Otros requerimientos no funcionales

### Requerimientos de rendimiento

ConectaITAM deberá mostrar el siguiente desempeño:
+ El sistema deberá de actualizarse en tiempo real.
+ Cualquier solicitud deberá responderse en menos de 500ms.
El desempeño dependerá del estado de los servidores y de la base de datos del ITAM.

### Requerimientos de seguridad (Safety)

ConectaITAM sigue los lineamientos de acuerdo a los estatutos de la institución. Por ello, nos apegamos a salvaguardar la integridad de nuestros usuarios y velar por su salud y seguridad personal.

+ **SA-1:** Se restringirá el lenguaje agresivo que los usuarios podrían usar durante sus conversaciones. 
+ **SA-2:** Se contará con una opción para notificar la revisión de menajes que puedieran agraviar a una persona.
+ **SA-3:** Se podrá bloquear la comunicación y denunciar al usuario haga mal uso de la herramienta.
+ **SA-4:** En casos extremos de acoso o agresión se podrá realizar una comunicación directa con un administrativo de servicios escolares adjuntando una copia de seguridad del chat del usuario que se está reportando.

### Requerimientos de seguridad (Security)

ConectaITAM sigue los lineamientos de privacidad y seguridad dictados por la institución. Por ello se siguen los siguientes requerimientos de protección, pues al ser una aplicación de chat para los asuntos escolares del ITAM, nos vemos en la necesidad de proteger la confidencialidad que la institución siempre ha protegido.

+ **SE-1:** Todos los usuarios de la aplicación serán validados directamente por la institución, de no ser así no podrán utilizar el sistema.
+ **SE-2:** Se manejará una lista de dispositivos de confianza para todos los usuarios.
+ **SE-3:** El inicio de sesión en nuevo dispositivo tendrá que realizar una verificación de dos pasos y se podrá marcar si este nuevo dispositivo será o no de confianza.
+ **SE-4:** La información sensible de los usuarios será protegida y encriptada, para proteger de cualquier robo de información o ataque.
+ **SE-5:** Los mensajes, tanto privados como públicos, serán encriptados para mantener la confidencialidad de los asuntos escolares de la institución.
+ **SE-6:** Se realizará constantemente copias de seguridad para mantener la integridad y confiabilidad de la base de datos.
+ **SE-7:** Los alumnos, no podrán gestionar de ninguna forma los grupos predefinidos por los administradores del sistema.
+ **SE-8:** Los profesores, junto con los administradores serán los únicos en gestionar los grupos predefinidos.

### Atributos de calidad de software

+ **SQ-1:** El sistema será fácil de usar para todos los usuarios, se aplicarán periodicamente un sondeo sobre usuarios seleccionados para evaluar nuestra calidad de diseño.
+ **SQ-2:** El sistema estará siempre disponible, teniendo principal cuidado en las horas pico. Por ello se monitorizarán constantemente las transacciones de datos y los incidentes que podrían llegar a suceder.
+ **SQ-3:** El sistema contará con constantes copias de seguridad de las versiones más estables para que en el caso de fallas se pueda mantener el servicio a nuestros usuarios.

### Reglas de negocio

+ **BU-1:** Solo los profesores y los administradores del sistema serán capaces de modificar los chats grupales predefinidos.
+ **BU-2:** Solo el administrador del sistema será capaz de bloquear permanentemente la comunicación entre dos usuarios.
+ **BU-3:** Solo los administradores de servicios escolares podrán gestionar la información del chatbot.
+ **BU-4:** Los estudiantes serán capaces de bloquear, como máximo una semana, la comunicación con otro usuario.

# 2. Plan de Calidad

## Identificador del plan de prueba

ComunicaITAM_1.0_Testing_Y4M3A8URR1

## Referencias

Los documentos que respaldan este plan de calidad son:

+ [Plan de proyecto y requerimientos del sistema](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#1-requerimientos-del-sistema)

## Introducción

Este plan de calidad para el sistema ConectaITAM se llevará acabo en los más populares navegadores web, tal como: Chrome, Firefox, Safari y Opera. En este documento se tendrá como objetivo:

+ Definir las herramientas para utiliar durante todo el proceso de pruebas.
+ Definir cuales son los parámetros para realizar dichas pruebas.
+ Identificar los elementos en los que se realiarán las pruebas y establecer lo que se espera de ellas.

Todo lo anterior para poder dar la mayor seguridad y confiabilidad a nuestro sistema de mensajería ConectaITAM.

## Elementos de prueba

Los elementos a probar del sistema ComunicaITAM son:

+ Inicio de sesión (con verificación)
+ Enviar y recibir mensajes entre usuarios.
+ Creación de chats grupales predefinidos.
+ Creación de chats grupales por los estudiantes.
+ Iniciar una nueva conversación.
+ Busqueda de usuario por nombre, correo instituciones o clase conjunta.
+ Gestión de conversaciones y de grupos privados.
+ Comunicación con el chatbot de servicios escolares.
+ Reporte de mensajes o de usuarios inapropiados.
+ Bloqueo de usuarios.

Los elementos deben probarse en Windows y MacOs, así como en los navegadores web más populares.

## Problemas de riesgo del software

Las áreas críticas del sistema ComunicaITAM son:

+ ...
+ 

## Funcionalidades a probar

+ Como estudiante/ profesor quiero ingresar al sistema ConectaITAM.
+ Como estudiante/profesor quiero navegar entre mis conversaciones.
+ Como estudiante/profesor quiero crear una nueva conversación.
+ Como estudiante/profesor quiero buscar a un usuario.
+ Como estudiante quiero crear un subgrupo de una materia.
+ Como estudiante/profesor quiero gestionar mis conversaciones.
+ Como estudiante/profesor quiero reportar a un usuario.
+ Como estudiante/profesor quiero envía un mensaje a una conversación ya creada.
+ Como estudiante quiero conversar con el chatbot de servicios escolares.
+ Como estudiante/profesor quiero subir un archivo multimedia.

## Funcionalidades que no deben probarse

Las siguientes funciones no serán sometidas a pruebas.

+ Notificación de nuevos mensajes.
+ Creación de chat grupales predefinidos.
+ Creación de agendar una cita por medio del chatbot.

## Enfoque (Estrategia) - ¡¡FALTA!!



## Críterios de aprobación/falla

El sistema ComunicaITAM seguirá los siguientes críterios de aprobación y falla:

+ Todas las funcionalidades del sistema descritos en este documento deben de funcionar de la manera en la que se tiene esperado y como se describe en el documento de requisitos.
+ No se aceptarán bajo ninguna circunstancia errores críticos ni defectos que se lleguen a encontrar durante el proceso de pruebas.
+ El estudiante debe de ser capaz de envía y recibir mensajes, crear y administrar sus conversaciones privadas, buscar usuarios, subir archivos multimedia y conversar con el chatbot. Todas las acciones se deben de poder acompletar sin retraso ni errores.
+ El profesor debe ser capaz de envía y recibir mensajes, crear y administrar sus conversaciones privadas, grationar los chat grupales predefinidos, buscar usuarios, subir archivos multimedia y conversar con el chatbot. Todas las acciones se deben de poder acompletar sin retraso ni errores.

## Criterios de suspensión y requisitos de reanudación

Las pruebas para el sistema ComunicaITAM deberán detenerse inmediatemente si:

+ Se experimenta error en inicio de sesión.
+ Se experimenta error en alguna acción básica como: creación, lectura, actualización y eliminación de solicitudes a la base de datos.
+ Existe un gran porcentaje de ciclos de prueba fallidos, más del 50% del total de los casos.
+ Se incrementa notablemente el número de defectos encontrados durante las pruebas, más de 10 defectos.

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




