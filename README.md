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

1. [Requrimientos del
   Sistema](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#1-requerimientos-del-sistema)
    1. [Introducción](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#11-introducción)
    2. [Descripción
       general](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#12-descripción-general)
    3. [Requerimientos de interfaz
       externa](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#13-requerimientos-de-interfaz-externa)
    4. [Funcionalidades del
       sistema](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#14-funcionalidades-del-sistema)
    5. [Otros requerimientos no
       funcionales](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#15-otros-requerimientos-no-funcionales)
2. [Plan de
   Calidad](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#2-plan-de-calidad)
    1. [Identificador del plan de
       prueba](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#21-identificador-del-plan-de-prueba)
    2. [Referencias](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#22-referencias)
    3. [Introducción](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#23-introducción)
    4. [Elementos de
       prueba](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#24-elementos-de-prueba)
    5. [Problemas de riesgo del
       software](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#25-problemas-de-riesgo-del-software)
    6. [Funcionalidades a
       probar](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#26-funcionalidades-a-probar)
    7. [Funcionalidades que no deben
       probarse](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#27-funcionalidades-que-no-deben-probarse)
    8. [Enfoque](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#28-enfoque)
    9. [Criterios de
       aprobación/falla](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#29-criterios-de-aprobación/falla)
    10. [Criterios de suspensión y requisitos de
        reanudación](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#210-criterios-de-suspensión-y-requisitos-de-reanudación)
    11. [Entregables de
        prueba](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#211-entregables-de-prueba)
    12. [Tareas de pruebas
        restantes](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#212-tareas-de-pruebas-restantes)
    13. [Necesidades
        ambientales](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#213-necesidades-ambientales)
    14. [Necesidades del personal y
        capacitación](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#214-necesidades-del-personal-y-capacitación)
    15. [Responsabilidades](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#215-responsabilidades)
    16. [Calendario](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#216-calendario)
    17. [Planificación de riesgos y
        contingencias](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#217-planificación-de-riesgos-y-contingencias)
    18. [Aprobación](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#218-aprobación)
    19. [Glosario](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#219-glosario)
3. [Arquitectura](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#3-arquitectura)
4. [Metodología](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#4-metodología)
5. [Instrucciones para
   replicar](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#5-instrucciones-para-replicar)
6. [Presentación](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#6-presentación)

# 1. Requerimientos del Sistema

## 1.1 Introducción

### Propósito

En este documento se describen las especificaciones de los requerimientos del sistema ConectaITAM,
la cual es una plataforma de comunicación exclusiva para el Instituto Tecnológico Autónomo de México
(ITAM). ConectaITAM provee un medio para que los alumnos del ITAM puedan comunicarse entre ellos,
así como también poder entablar conversaciones con profesores y con el personal
administrativo. ConectaITAM tiene como objetivo mejorar la experiencia de los estudiantes,
facilitándoles las herramientas para poder expresarse y desarrollarse de la mejor manera en su vida
diaria como estudiantes. A continuación, se describe detalladamente la plataforma de ConectaITAM
1.0.

### Convenciones del documento

En este documento se hace uso del estándar de la IEEE para SRS (_Software Requirements
Specifications_), SIO/IEC/IEEE 29148.

En la asignación de prioridades para las funcionalidades del _software_, se maneja un rango de 1 a
3, en el cual 1 significa que el requerimiento es indispensable y 3 denota que se puede prescindir
de él.

### Público objetivo y sugerencicas de lectura

Este documento está dirigido hacia los desarrolladores que están a cargo del mantenimiento del
sistema ConectaITAM. Se espera que este cuerpo de desarrolladores se conforme por el personal
administrativo del área de cómputo en el ITAM. Se les sugiere leer todo el documento y
posteriormente apoyarse en el índice para referenciar rápidamente las secciones relevantes que se
requieran para el mantenimiento del sistema.

### Alcance del producto

ConectaITAM es una plataforma que permite a los alumnos del ITAM tener una aplicación para la
comunicación rápida y eficaz con todos los estudiantes, profesores y personal administrativo del
ITAM.

ConectaITAM tiene como metas:
- Proporcionar un nuevo medio para la comunicación entre toda la comunidad, el cual va más allá del
  correo electrónico institucional.
- Llegar a ser la principal vía de comunicación para los asuntos escolares dentro de la comunidad.
- Mejorar las relaciones alumno-profesor, alumno-personal administrativo y alumno-alumno.
- Mejorar la experiencia de vida institucional.
    + Los alumnos tendrán un medio para obtener fácilmente información relevante a las dudas que
      puedan tener, tanto de una clase como de los asuntos administrativos.
    + Los profesores tendrán un medio para difundir mensajes urgentes como avisos de imprevistos o
      cambios de fechas, así como para ofrecer ayuda personalizada dirigida a los alumnos en sus
      clases.
    + Los administrativos podrán ofrecer información general por medio de un _chatbot_, evitando que
      los alumnos tengan que acudir a las instalaciones para tareas sencillas, lo cual reducirá la
      carga administrativa.

## 1.2 Descripción general

### Perspectiva del producto

ConectaITAM es una plataforma que será añadida al conjunto de aplicaciones ofrecidas por el ITAM.
La plataforma busca complementar a las aplicaciones ya existentes, tal como Comunidad ITAM y
Servicios Web.

A continuación, se muestra un diagrama que ilustra las entidades externas y los actores del sistema.

![](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/mapa1.png)

### Funciones del producto

El sistema ConectaITAM ofrece las siguientes funcionalidades principales:

+ **PF-1:** Almacenar y ofrecer en tiempo real las conversaciones de cada usuario del sistema.
+ **PF-2:** Buscar usuarios a través de su nombre, correo institucional y en la lista de alumnos y
  profesores de una clase.
+ **PF-3:** Enviar mensajes directos y archivos multimedia a otros usuarios.
+ **PF-4:** Crear y gestionar conversaciones grupales privadas, de una clase o de un grupo de
  alumnos arbitrario.
+ **PF-5:** Crear y gestionar conversaciones individuales entre alumnos y profesores.
+ **PF-6:** Gestionar y ofrecer conversaciones del _chatbot_ asistente de servicios escolares y
  departamentos académicos.
+ **PF-7:** Crear y gestionar conversaciones con el personal de servicios escolares y departamentos
  académicos.

### Clases y características del usuario

Los tipos de usuario que utilizarán ConectaITAM son:

+ **Administradores:** Grupo encargado de administrar y mantener la plataforma ConectaITAM, incluída
  la base de datos y los sistemas relacionados a esta. Se espera en un inicio gran interación con la
  plataforma, dado que son los encargados de la gestión de chats grupales predefinidos relacionados
  a las clases inscritas del alumno, así como de la gestión del _chatbot_. Se espera que los
  administradores tengan un alto conocimiento del software.
+ **Estudiantes:** Serán los usuarios que tendrán mayor contacto con la plataforma; se espera un uso
  diario. Se considera estudiante a todo aquel que curse alguna materia en el ITAM, sea de
  licenciatura, ingeniería o algún posgrado. Se esperan las siguientes interacciones: enviar y
  recibir mensajes, crear y gestionar chats grupales y buscar usuarios.
+ **Personal administrativo:** Se espera un menor contacto del personal administrativo, pues el
  objetivo es disminuir su trabajo mediante el _chatbot_. Se considera personal administrativo a
  todas aquellas personas que pertenecen a Servicios Escolares, así como a los administrativos de
  los departamentos acádemicos. Se esperan las siguientes interacciones: dar información tanto
  general como personalizada a los alumnos; brindar apoyo y resolver dudas sobre su vida académica,
  y; enviar y recibir mensajes de otros usuarios cuando sea necesario.
+ **Profesores:** Serán los usuarios con la segunda mayor interacción con la plataforma. Se
  consideran profesores a todos los catedráticos que se encuentren impartiendo alguna clase en la
  institución. Se esperan las siguientes interacciones: enviar y recibir mensajes con otros
  usuarios, buscar usuarios y enviar mensajes urgentes.

### Entorno operativo

ConectaITAM está desarrollado para poder operar en el siguiente entorno: 
+ **OE-1:** No hay restricción geográfica de dónde funcionará la plataforma.
+ **OE-2:** Deberá ser accesible mediante los navegadores _web_ principales: Chrome, Firefox, Safari y
  Opera.
+ **OE-3:** Se deberá proporcionar un servicio continuo y estable.

### Restricciones de diseño e implementación

ConectaITAM está restringido por las siguientes limitaciones:
+ **DIC-1:** Se deberán cumplir las políticas de información, seguridad y privacidad del ITAM.
+ **DIC-2:** Se deberán usar las tecnologías de acuerdo a los estándares del ITAM.
+ **DIC-3:** Se limitará el tamaño de los archivos multimedia compartidos mediante el chat.
+ **DIC-4:** Se limitará el tipo de archivos multimedia compartidos mediante el chat.
+ **DIC-5:** No habrá soporte para llamadas ni videollamadas.

### Documentación del usuario

ConectaITAM proveerá dos tipos de apoyo para sus usuarios.
+ Dentro de la plataforma habrá un botón de ayuda, el cual incluirá un tutorial interactivo para los
  usuarios.
+ Fuera de la plataforma, el ITAM proveerá un manual de usuario en su portal principal.
    - Este manual de usuario será envíado también a través del correo institucional cuando la
      aplicación entre en uso.

### Suposiciones y dependencias

ConectaITAM cuenta con las siguientes dependencias:
+ **AS-1:** Las cuentas de usuarios de la plataforma están ligadas a la autenticación del
  ITAM. Ninguna persona que no posea un correo institucional verificado podrá tener acceso a la
  aplicación.
+ **AS-2:** Queda sujeta al funcionamiento de los servidores y de la base de datos del ITAM.
+ **AS-3:** Asume que la plataforma podrá funcionar adecuadamente con aproximadamente 6,000
  usuarios.
+ **AS-4:** Presume que los usuarios tendrán actualizados sus sistemas operativos y navegadores web.

## 1.3 Requerimientos de interfaz externa

### Interfaces de usuario

### Interfaces de hardware

### Interfaces de software

### Interfaces de comunicaciones

## 1.4 Funcionalidades del sistema

### Iniciar sesión 

#### Descripción
Esta es la funcionalidad con mayor prioridad (1) en este proyecto porque de esta depende que el
usuario pueda hacer uso de las demás funcionalidades. Solamente miembros de la comunidad ITAM con
una dirección de correo válida podrán crear una cuenta en la plataforma; habrá una verificación de
la misma.

#### Estímulos / Respuestas

#### Requerimientos funcionales
+ **REQ-1**: La plataforma deberá contar con un sistema para la verificación de correo.
+ **REQ-2**: Debe existir un sistema de búsqueda siempre accesible al usuario.

### Creación de conversaciones grupales

#### Descripción
Esta no es una función tan relevante para nuestro sistema dado que los alumnos ya tienen un gran
número de herramientas para comunicarse entre sí. Sin embargo, es importante para los proyectos
grupales y otras comunicaciones. Por esta razón, se le dio una prioridad baja (3).

#### Estímulos / Respuestas

#### Requerimientos funcionales
+ **REQ-1**: Los alumnos que sean invitados a la conversación grupal tendrán que existir en
  ConectaITAM.
+ **REQ-2**: Deberá existir una categoría de conversación grupal en la plataforma.

### Buscar contacto

#### Descripción
Se le asignó una prioridad media (2) a esta funcionalidad, pues es necesaria para la creación de los
grupos. Asimismo, es importante que un alumno pueda buscar un contacto en caso de no tener ningún
otro medio para comunicarse.

#### Estímulos / Respuestas

#### Requerimientos funcionales
+ **REQ-1**: El sistema debe desplegar, en orden descendiente por grupos en común, los resultados de
  la búsqueda.
+ **REQ-2**: 

### Comunicarse con un profesor

#### Descripción
Esta es una funcionalidad muy importante de la plataforma (1) puesto que, al ser una aplicación
universitaria, la comunicación entre alumnos y profesores es vital.

#### Estímulos / Respuestas
+ Estímulo: El alumno seleccionará un profesor para mandarle un mensaje.

+ Respuesta: El sistema enviará el mensaje junto con una notificación al profesor seleccionado.

#### Requerimientos funcionales
+ **REQ-1**: El alumno debe estar inscrito en al menos una materia con el profesor con el cual
  quiere comunicarse.
+ **REQ-2**: 

### Reportar un mal funcionamiento de la aplicación

#### Descripción
El usuario puede ver un mal funcionamiento de la aplicación y querrá reportarlo para que pueda ser
arreglado. Por ser una funcionalidad que reportará sobre el buen funcionamiento de la aplicación, se
asigna prioridad media (2).

#### Estímulos / Respuestas
+ Estímulo: El usuario nota que una funcionalidad está fallando, decide levantar un reporte con el botón de
reporte. 

+ Respuesta: El sistema registra este reporte y se manda un mensaje de confirmación y agradecimiento.

#### Requerimientos funcionales
+ **REQ-1**: Debe haber un botón apropiado para realizar esta acción.
+ **REQ-2**: El sistema debe tener una base de datos para los reportes de mal funcionamientos.

## 1.5 Otros requerimientos no funcionales

### Requerimientos de rendimiento

ConectaITAM deberá mostrar el siguiente desempeño:
+ El sistema deberá actualizarse automáticamente en cuanto sea posible.
+ Cualquier solicitud deberá ser satisfecha en menos de 500ms. El desempeño dependerá de la carga en
los servidores y en la base de datos del ITAM.

### Requerimientos de seguridad (Safety)

ConectaITAM se apega al reglamento de alumnos, de profesores y de administrativos de la
institución. Por ello, está sujeto a salvaguardar la integridad de los usuarios y proteger su
bienestar y seguridad personal.

+ **SA-1:** Se reportará y penalizará el lenguaje agresivo que los usuarios empleen durante sus
  conversaciones.
+ **SA-2:** Se contará con una opción que marque para revisión manual los mensajes que agredan a un
  usuario.
+ **SA-3:** Se podrá bloquear la comunicación con un usuario y denunciarle por hacer mal uso de la
  herramienta.
+ **SA-4:** En casos extremos de acoso o agresión, se podrá solicitar una comunicación directa con
  un administrativo de servicios escolares, adjuntando una copia de seguridad de la conversación con
  el usuario agresor.

### Requerimientos de seguridad (Security)

ConectaITAM sigue los lineamientos de privacidad y seguridad dictados por la institución. Por ello,
se siguen los siguientes requerimientos de protección. Al ser una plataforma de comunicación para
los asuntos escolares del ITAM, es necesario proteger la confidencialidad que la institución es
responsable de salvaguardar.

+ **SE-1:** Todos los usuarios de la aplicación serán validados directamente por la institución. De
  no ser así, no podrán utilizar el sistema.
+ **SE-2:** Se manejará una lista de dispositivos de confianza para todos los usuarios.
+ **SE-3:** Al iniciar sesión en nuevo dispositivo, se deberá verificar el mismo y el sistema
  establecerá la confianza del nuevo equipo.
+ **SE-4:** La información sensible de los usuarios será protegida y encriptada para defenderse de
  cualquier robo de información o ataque.
+ **SE-5:** Los mensajes, tanto privados como públicos, serán encriptados para mantener la
  confidencialidad de los asuntos escolares de la institución.
+ **SE-6:** Se realizarán constantemente copias de seguridad para mantener la integridad y
  confiabilidad de la base de datos.
+ **SE-7:** Los alumnos no podrán gestionar de ninguna forma los grupos predefinidos por los
  administradores del sistema.
+ **SE-8:** Los profesores, junto con los administradores, serán los únicos que gestionen los grupos
  predefinidos.

### Atributos de calidad de software

+ **SQ-1:** El sistema será fácil de usar para todos los usuarios, se aplicará periodicamente un
sondeo a usuarios seleccionados para evaluar la calidad de diseño.

+ **SQ-2:** El sistema estará siempre disponible, con un enfoque en las horas pico. Por ello ,se
monitorearán constantemente las transacciones de datos y los incidentes que podrían llegar a
suceder.

+ **SQ-3:** El sistema contará con frecuentes copias de seguridad de los estados estables del mismo,
para que en el caso de fallas, se pueda reestablecer el servicio a los usuarios.

### Reglas de negocio

+ **BU-1:** Solo los profesores y los administradores del sistema serán capaces de modificar los
chats grupales predefinidos.

+ **BU-2:** Solo los administradores del sistema serán capaces de bloquear permanentemente la
comunicación entre dos usuarios.

+ **BU-3:** Solo los administrativos de servicios escolares y departamentos académicos, así como los
administradores, podrán gestionar la información del chatbot.

+ **BU-4:** Los estudiantes serán capaces de bloquear, por una semana como máximo, la comunicación
con otro usuario.

# 2. Plan de Calidad

## 2.1 Identificador del plan de prueba

ComunicaITAM\_1.0\_Testing\_Y4M3A8URR1

## 2.2 Referencias

Los documentos que respaldan este plan de calidad son:

[Plan de proyecto y requerimientos del
sistema](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/README.md#1-requerimientos-del-sistema)

## 2.3 Introducción

Este plan de calidad para la plataforma ConectaITAM está elaborado en torno a los más populares
navegadores _web_, tal como: Chrome, Firefox, Safari y Opera. En este documento se tiene como
objetivo:

+ Definir las herramientas para utiliar durante todo el proceso de pruebas.
+ Definir cuales son los parámetros para realizar dichas pruebas.
+ Identificar los elementos sobre los cuales se realizarán las pruebas y establecer lo que se espera
  de ellas.

Todo lo anterior se define con el fin de dar la mayor seguridad y confiabilidad a la plataforma de
comunicación ConectaITAM.

## 2.4 Elementos de prueba

Los elementos a probar del sistema ConectaITAM son:

+ Iniciar sesión (con verificación).
+ Enviar y recibir mensajes entre usuarios.
+ Crear conversaciones grupales predefinidss.
+ Crear conversaciones grupales como estudiante.
+ Crear una nueva conversación individual.
+ Buscar usuarios por nombre, correo institucional o lista de alumnos y profesores de la clase.
+ Gestionar conversaciones y grupos privados.
+ Establecer comunicaciones con el _chatbot_ de servicios escolares y departamentos académicos.
+ Reportar mensajes o a usuarios inapropiados.
+ Bloquear usuarios.

## 2.5 Problemas de riesgo del software

Las áreas críticas del sistema ConectaITAM son:

+ Intercambio de mensajes a través de la red.
+ Almacenamiento de conversaciones, datos personales y demás información confidencial.
+ Envío de archivos multimedia.
+ Permisos de administradores, profesores y empleados administrativos.

## 2.6 Funcionalidades a probar

A cada funcionalidad se le asigna un riesgo en el rango de 1 a 3, siendo 1 el mayor riesgo y 3 el
menor.

+ (1) Como estudiante/profesor quiero ingresar al sistema ConectaITAM.
+ (2) Como estudiante/profesor quiero visualizar y entrar a mis conversaciones.
+ (3) Como estudiante/profesor quiero crear una nueva conversación.
+ (3) Como estudiante/profesor quiero buscar a un usuario.
+ (3) Como estudiante quiero crear un subgrupo de una materia.
+ (2) Como estudiante/profesor quiero gestionar mis conversaciones.
+ (2) Como estudiante/profesor quiero reportar a un usuario.
+ (3) Como estudiante/profesor quiero enviar un mensaje a una conversación ya creada.
+ (2) Como estudiante quiero conversar con el _chatbot_ de servicios escolares y departamentos
  académicos.
+ (1) Como estudiante/profesor quiero compartir un archivo multimedia.

## 2.7 Funcionalidades que no deben probarse

Las siguientes funciones no serán sometidas a pruebas.

+ Enviar notificaciones de nuevos mensajes.
+ Crear conversaciones grupales predefinidas.
+ Agendar una cita por medio del chatbot.

## 2.8 Enfoque (estrategia)

+ La plataforma debe probarse en Windows, MacOS y Linux, así como en los navegadores web más
  populares (Chrome, Firefox, Safari y Opera).

## 2.9 Criterios de aprobación/falla

El sistema ConectaITAM seguirá los siguientes críterios de aprobación y falla:

+ Todas las funcionalidades del sistema descritas en este documento deben de funcionar de la manera
  en la que se espera y como se describe en el documento de requisitos.
+ No se aceptarán bajo ninguna circunstancia errores críticos ni defectos que se encuentren durante
  el proceso de pruebas.
+ El estudiante debe de ser capaz de enviar y recibir mensajes, crear y administrar sus
  conversaciones privadas, buscar usuarios, subir archivos multimedia y conversar con el
  _chatbot_. Todas las acciones se deben efectuar con retrasos o errores mínimos.
+ El profesor debe ser capaz de enviar y recibir mensajes, crear y administrar sus conversaciones
  privadas, gestionar las conversaciones grupales predefinidas, buscar usuarios, subir archivos
  multimedia y conversar con el _chatbot_.  Todas las acciones se deben efectuar con retrasos o
  errores mínimos.

## 2.10 Criterios de suspensión y requisitos de reanudación

Las pruebas para el sistema ConectaITAM deberán detenerse inmediatemente si:

+ Se experimenta error en inicio de sesión.
+ Se experimenta error en alguna acción básica como: creación, lectura, actualización y eliminación
  de solicitudes a la base de datos.
+ Existe un gran porcentaje de ciclos de prueba fallidos (más del 50% del total de los casos).
+ Incrementan notablemente el número de defectos encontrados durante las pruebas (más de 10
  defectos).

## 2.11 Entregables de prueba

## 2.12 Tareas de pruebas restantes

## 2.13 Necesidades ambientales

## 2.14 Necesidades del personal y capacitación

## 2.15 Responsabilidades

## 2.16 Calendario

## 2.17 Planificación de riesgos y contingencias

## 2.18 Aprobación

## 2.19 Glosario

# 3. Arquitectura

ConectaITAM utiliza una arquitectura por eventos. Las características de la arquitectura para esta
plataforma ofrecen ventajas sobre las demás arquitecturas, con las menores desventajas. Asimismo, el
uso que le darán los usuarios a la plataforma será en forma de eventos, puesto que dichos usuarios
no entablan una comunicación constante con otros usuarios, sino cuando lo demandan, y el sistema
deberá responder en dicho caso.

# 4. Metodología

ConectaITAM sigue una metodología incremental. La plataforma está suficientemente bien definida para
seguir una metodología de cascada, pero la metodología incremental permite la atomización del
proyecto para un desarrollo más fluido.  Además, es importante emprender las tareas con más alta
prioridad sin dejar a un lado el proyecto en su totalidad.

Otra ventaja de la metodología es que permite presentar un producto inicial a un bajo costo y en un
periodo corto de tiempo. Después de la presentación inicial del producto, los defectos o *bugs* son
fáciles de detectar, dado que los cambios desde el último incremento son relativamente pequeños.

# 5. Instrucciones para replicar

# 6. Presentación

Podrá encontrar la presentación del proyecto final [aquí]()




