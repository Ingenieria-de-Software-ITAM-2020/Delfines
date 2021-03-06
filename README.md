![](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/encabezado.png)

![](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/logo.png)

**Proyecto Final: ConectaITAM** 

**Equipo:** Delfines en Éxtasis

**Integrantes:**
- Jacqueline Lira Chávez - 167334
- José Luis Sandín Espinosa - 179706
- Mónica Hernández Martínez - 163543
- Piero Vera Stephens - 179915

**Liga:** [ConectaITAM](https://jacquelinelira.github.io/ConectaItam/)

# Índice


- [Requerimientos del Sistema](#requerimientos-del-sistema)
  * [1 Introducción](#1-introducción)
    + [1.1 Propósito](#11-propósito)
    + [1.2 Convenciones del documento](#12-convenciones-del-documento)
    + [1.3 Público objetivo y sugerencicas de lectura](#13-público-objetivo-y-sugerencicas-de-lectura)
    + [1.4 Alcance del producto](#14-alcance-del-producto)
  * [2 Descripción general](#2-descripción-general)
    + [2.1 Perspectiva del producto](#21-perspectiva-del-producto)
    + [2.2 Funciones del producto](#22-funciones-del-producto)
    + [2.3 Clases y características del usuario](#23-clases-y-características-del-usuario)
    + [2.4 Entorno operativo](#24-entorno-operativo)
    + [2.5 Restricciones de diseño e implementación](#25-restricciones-de-diseño-e-implementación)
    + [2.6 Documentación del usuario](#26-documentación-del-usuario)
    + [2.7 Suposiciones y dependencias](#27-suposiciones-y-dependencias)
  * [3 Requerimientos de interfaz externa](#3-requerimientos-de-interfaz-externa)
    + [3.1 Interfaces de usuario](#31-interfaces-de-usuario)
    + [3.2 Interfaces de hardware](#32-interfaces-de-hardware)
    + [3.3 Interfaces de software](#33-interfaces-de-software)
    + [3.4 Interfaces de comunicaciones](#34-interfaces-de-comunicaciones)
  * [4 Funcionalidades del sistema](#4-funcionalidades-del-sistema)
    + [4.1 Iniciar sesión](#41-iniciar-sesión)
      - [4.1.1 Descripción](#411-descripción)
      - [4.1.2 Estímulos / Respuestas](#412-estímulos-respuestas)
      - [4.1.3 Requerimientos funcionales](#413-requerimientos-funcionales)
    + [4.2 Enviar mensajes individuales](#42-enviar-mensajes-individuales)
      - [4.2.1 Descripción](#421-descripción)
      - [4.2.2 Estímulos / Respuestas](#422-estímulos-respuestas)
      - [4.2.3 Requerimientos funcionales](#423-requerimientos-funcionales)
    + [4.3 Comunicarse con un profesor](#43-comunicarse-con-un-profesor)
      - [4.3.1 Descripción](#431-descripción)
      - [4.3.2 Estímulos / Respuestas](#432-estímulos-respuestas)
      - [4.3.3 Requerimientos funcionales](#433-requerimientos-funcionales)
    + [4.4 Subir archivos multimedia](#44-subir-archivos-multimedia)
      - [4.4.1 Descripción](#441-descripción)
      - [4.4.2 Estímulos / Respuestas](#442-estímulos-respuestas)
      - [4.4.3 Requerimientos funcionales](#443-requerimientos-funcionales)
    + [4.5 Reportar un mal funcionamiento de la aplicación](#45-reportar-un-mal-funcionamiento-de-la-aplicación)
      - [4.5.1 Descripción](#451-descripción)
      - [4.5.2 Estímulos / Respuestas](#452-estímulos-respuestas)
      - [4.5.3 Requerimientos funcionales](#453-requerimientos-funcionales)
    + [4.6 Buscar contacto](#46-buscar-contacto)
      - [4.6.1 Descripción](#461-descripción)
      - [4.6.2 Estímulos / Respuestas](#462-estímulos-respuestas)
      - [4.6.3 Requerimientos funcionales](#463-requerimientos-funcionales)
    + [4.7 Creación de conversaciones grupales](#47-creación-de-conversaciones-grupales)
      - [4.7.1 Descripción](#471-descripción)
      - [4.7.2 Estímulos / Respuestas](#472-estímulos-respuestas)
      - [4.7.3 Requerimientos funcionales](#473-requerimientos-funcionales)
  * [5 Otros requerimientos no funcionales](#5-otros-requerimientos-no-funcionales)
    + [5.1 Requerimientos de rendimiento](#51-requerimientos-de-rendimiento)
    + [5.2 Requerimientos de seguridad (Safety)](#52-requerimientos-de-seguridad-safety)
    + [5.3 Requerimientos de seguridad (Security)](#53-requerimientos-de-seguridad-security)
    + [5.4 Atributos de calidad de software](#54-atributos-de-calidad-de-software)
    + [5.5 Reglas de negocio](#55-reglas-de-negocio)
- [Plan de Calidad](#plan-de-calidad)
  * [1 Identificador del plan de prueba](#1-identificador-del-plan-de-prueba)
  * [2 Referencias](#2-referencias)
  * [3 Introducción](#3-introducción)
  * [4 Elementos de prueba](#4-elementos-de-prueba)
  * [5 Problemas de riesgo del software](#5-problemas-de-riesgo-del-software)
  * [6 Funcionalidades a probar](#6-funcionalidades-a-probar)
  * [7 Funcionalidades que no deben probarse](#7-funcionalidades-que-no-deben-probarse)
  * [8 Enfoque (estrategia)](#8-enfoque-estrategia)
  * [9 Criterios de aprobación/falla](#9-criterios-de-aprobación-falla)
  * [10 Criterios de suspensión y requisitos de reanudación](#10-criterios-de-suspensión-y-requisitos-de-reanudación)
  * [11 Entregables de prueba](#11-entregables-de-prueba)
  * [12 Tareas de pruebas restantes](#12-tareas-de-pruebas-restantes)
  * [13 Necesidades ambientales](#13-necesidades-ambientales)
  * [14 Necesidades del personal y capacitación](#14-necesidades-del-personal-y-capacitación)
  * [15 Responsabilidades](#15-responsabilidades)
  * [16 Calendario](#16-calendario)
  * [17 Planificación de riesgos y contingencias](#17-planificación-de-riesgos-y-contingencias)
  * [18 Aprobación](#18-aprobación)
- [Arquitectura](#arquitectura)
- [Metodología](#metodología)
- [Casos de Uso](#casos-de-uso)
- [Instrucciones para replicar](#instrucciones-para-replicar)
- [Presentación](#presentación)

# Requerimientos del Sistema

## 1 Introducción

### 1.1 Propósito

En este documento se describen las especificaciones de los requerimientos del sistema ConectaITAM,
la cual es una plataforma de comunicación exclusiva para el Instituto Tecnológico Autónomo de México
(ITAM). ConectaITAM provee un medio para que los alumnos del ITAM puedan comunicarse entre ellos,
así como también poder entablar conversaciones con profesores y con el personal
administrativo. ConectaITAM tiene como objetivo mejorar la experiencia de los estudiantes,
facilitándoles las herramientas para poder expresarse y desarrollarse de la mejor manera en su vida
diaria como estudiantes. A continuación, se describe detalladamente la plataforma de ConectaITAM
1.0.

### 1.2 Convenciones del documento

En este documento se hace uso del estándar de la IEEE para SRS (_Software Requirements
Specifications_), SIO/IEC/IEEE 29148.

En la asignación de prioridades para las funcionalidades del _software_, se maneja un rango de 1 a
3, en el cual 1 significa que el requerimiento es indispensable y 3 denota que se puede prescindir
de él.

### 1.3 Público objetivo y sugerencicas de lectura

Este documento está dirigido hacia los desarrolladores que están a cargo del mantenimiento del
sistema ConectaITAM. Se espera que este cuerpo de desarrolladores se conforme por el personal
administrativo del área de cómputo en el ITAM. Se les sugiere leer todo el documento y
posteriormente apoyarse en el índice para referenciar rápidamente las secciones relevantes que se
requieran para el mantenimiento del sistema.

### 1.4 Alcance del producto

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

## 2 Descripción general

### 2.1 Perspectiva del producto

ConectaITAM es una plataforma que será añadida al conjunto de aplicaciones ofrecidas por el ITAM.
La plataforma busca complementar a las aplicaciones ya existentes, tal como Comunidad ITAM y
Servicios Web.

A continuación, se muestra un diagrama que ilustra las entidades externas y los actores del sistema.

![](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/mapa1.png)

### 2.2 Funciones del producto

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

### 2.3 Clases y características del usuario

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

### 2.4 Entorno operativo

ConectaITAM está desarrollado para poder operar en el siguiente entorno: 
+ **OE-1:** No hay restricción geográfica de dónde funcionará la plataforma.
+ **OE-2:** Deberá ser accesible mediante los navegadores _web_ principales: Chrome, Firefox, Safari y
  Opera.
+ **OE-3:** Se deberá proporcionar un servicio continuo y estable.

### 2.5 Restricciones de diseño e implementación

ConectaITAM está restringido por las siguientes limitaciones:
+ **DIC-1:** Se deberán cumplir las políticas de información, seguridad y privacidad del ITAM.
+ **DIC-2:** Se deberán usar las tecnologías de acuerdo a los estándares del ITAM.
+ **DIC-3:** Se limitará el tamaño de los archivos multimedia compartidos mediante el chat.
+ **DIC-4:** Se limitará el tipo de archivos multimedia compartidos mediante el chat.
+ **DIC-5:** No habrá soporte para llamadas ni videollamadas.

### 2.6 Documentación del usuario

ConectaITAM proveerá dos tipos de apoyo para sus usuarios.
+ Dentro de la plataforma habrá un botón de ayuda, el cual incluirá un tutorial interactivo para los
  usuarios.
+ Fuera de la plataforma, el ITAM proveerá un manual de usuario en su portal principal.
    - Este manual de usuario será envíado también a través del correo institucional cuando la
      aplicación entre en uso.

### 2.7 Suposiciones y dependencias

ConectaITAM cuenta con las siguientes dependencias:
+ **AS-1:** Las cuentas de usuarios de la plataforma están ligadas a la autenticación del
  ITAM. Ninguna persona que no posea un correo institucional verificado podrá tener acceso a la
  aplicación.
+ **AS-2:** Queda sujeta al funcionamiento de los servidores y de la base de datos del ITAM.
+ **AS-3:** Asume que la plataforma podrá funcionar adecuadamente con aproximadamente 6,000
  usuarios.
+ **AS-4:** Presume que los usuarios tendrán actualizados sus sistemas operativos y navegadores web.

## 3 Requerimientos de interfaz externa

### 3.1 Interfaces de usuario

La interfaz de usuario será muy intuitiva y agradable hacia el usuario. Será similar en
funcionamiento a otras aplicaciones que los alumnos han usado en el pasado.

### 3.2 Interfaces de hardware

Esta aplicación está orientada a los navegadores en ordenadores con sistemas operativos MacOS (OS X
10.10 o superior), Windows(Windows 7 o superior) y Linux.  Sin embargo, también funcionará en
dispositivos móviles Android (Pie o superior) y iOS (13 o superior)

### 3.3 Interfaces de software

El software necesario será alguno de los navegadores más populares tales como 
+ Chrome (version 87.0.4280.66 o superior), 
+ Firefox (version 81.0 o superior), 
+ Safari (Release 91 o superior)
+ Opera (Opera 63 o superior).

### 3.4 Interfaces de comunicaciones

Para que ConectaITAM funcione, es necesaria una conexión estable a internet con 10Mbps de *download*
y 2Mbps de *upload* o más.

## 4 Funcionalidades del sistema

### 4.1 Iniciar sesión 

#### 4.1.1 Descripción

+ **Prioridad:** 1

Esta es la funcionalidad con mayor prioridad en este proyecto porque de esta depende que el usuario
pueda hacer uso de las demás funcionalidades. Solamente miembros de la comunidad ITAM con una
dirección de correo válida podrán crear una cuenta en la plataforma; habrá una verificación de la
misma.

#### 4.1.2 Estímulos / Respuestas
+ Estímulo: El usuario ingresa sus credenciales y son correctas.
+ Respuesta: El sistema permititá el acceso a las demás funcionalidades.
+ Estímulo: El usuario ingresa credenciales incorrectas.
+ Respuesta: El sistema indicará que las credenciales son incorrectas. Después de tres intentos, el
usuario será bloqueado temporalmente de su cuenta.
+ Estímulo: El usuario ingresa desde un nuevo dispositivo.
+ Respuesta: El sistema deberá solicitarle al usuario que verifique su nuevo dispositivo.


#### 4.1.3 Requerimientos funcionales
+ **REQ-1**: La plataforma deberá contar con un sistema para la verificación de correo.

+ **REQ-2**: Debe existir un sistema de búsqueda siempre accesible al usuario.

### 4.2 Enviar mensajes individuales

#### 4.2.1 Descripción

+ **Prioridad:** 1

Esta funcionalidad tiene conjuntamente la mayor prioridad de toda la plataforma ya que es la base
del sistema de comunicación. Es necesario que para enviar mensajes, los usuarios tengan las cuentas
autorizadas y activadas.

#### 4.2.2 Estímulos / Respuestas
+ Estímulo: El usuario selecciona un contacto y le envía un mensaje.
+ Respuesta: El sistema entregará el mensaje al usuario y le notificará de ello.

#### 4.2.3 Requerimientos funcionales
+ **REQ-3**: La plataforma deberá almacenar las comunicaciones de los usuarios.

+ **REQ-4**: Los mensajes deberán ser enviados y se notificará al destinatario.

### 4.3 Comunicarse con un profesor

#### 4.3.1 Descripción

+ **Prioridad:** 1

Esta es una funcionalidad muy importante de la plataforma puesto que, al ser una aplicación
universitaria, la comunicación entre alumnos y profesores es vital.

#### 4.3.2 Estímulos / Respuestas
+ Estímulo: El alumno selecciona un profesor para mandarle un mensaje.

+ Respuesta: El sistema enviará el mensaje junto con una notificación al profesor seleccionado.

#### 4.3.3 Requerimientos funcionales
+ **REQ-5**: El alumno debe estar inscrito en al menos una materia con el profesor con el cual
  quiere comunicarse.
  
+ **REQ-6**: De no ser horario laboral, quedará a decisión del profesor recibir estos mensajes.

### 4.4 Subir archivos multimedia

#### 4.4.1 Descripción

+ **Prioridad:** 2

Los usuarios, para fines de sus clases, necesitan tener la habilidad de compartirse archivos
multimedia, por lo cual es una tarea importante de prioridad media. Esto, además, requerirá de
filtración por tipos de archivo.

#### 4.4.2 Estímulos / Respuestas

+ Estímulo: El usuario carga un archivo que desea compartir con otro usuario o grupo de usuarios.

+ Respuesta: El sistema verifica que el archivo sea aceptado, notifica al usuario y entrega el
  archivo como mensaje al destinatario.

#### 4.4.3 Requerimientos funcionales

+ **REQ-7**: Se debe contar con un sistema de almacenamiento de archivos multimedia por
  un periodo de tiempo razonable para ser descargados en una conversación.
  
+ **REQ-8**: Los archivos deberán ser analizados y filtrados internamente para verificar que el
  archivo sea legítimo y no malicioso.

### 4.5 Reportar un mal funcionamiento de la aplicación

#### 4.5.1 Descripción

+ **Prioridad:** 2

El usuario puede ver un mal funcionamiento de la aplicación y querrá reportarlo para que pueda ser
arreglado. Por ser una funcionalidad que reportará sobre el buen funcionamiento de la aplicación, se
asigna prioridad media.

#### 4.5.2 Estímulos / Respuestas
+ Estímulo: El usuario nota que una funcionalidad está fallando, decide levantar un reporte con el botón de
reporte y una breve descripción. 

+ Respuesta: El sistema registra este reporte y se manda un mensaje de confirmación y agradecimiento.

#### 4.5.3 Requerimientos funcionales
+ **REQ-9**: Debe haber un botón apropiado para realizar esta acción.

+ **REQ-10**: El sistema debe tener una base de datos para los reportes de mal funcionamientos.

### 4.6 Buscar contacto

#### 4.6.1 Descripción

+ **Prioridad:** 3

Se le asignó una prioridad baja a esta funcionalidad, pues no es necesaria para la creación de los
grupos predefinidos, únicamente para grupos arbitrarios. Sin embargo, es importante que un alumno
pueda buscar un contacto en caso de no tener ningún otro medio para comunicarse.

#### 4.6.2 Estímulos / Respuestas
+ Estímulo: El alumno introduce el nombre o dirección de correo electrónico del contacto que quiere
  buscar.

+ Respuesta: El sistema desplegará una lista de alumnos que coincidan con los parámetros
  introducidos por el usuario.

#### 4.6.3 Requerimientos funcionales
+ **REQ-11**: El sistema debe desplegar, en orden descendiente por grupos en común, los resultados de
  la búsqueda.
  
+ **REQ-12**: Se desplegará un mensaje adecuado con respecto a los resultados de la búsqueda.

### 4.7 Creación de conversaciones grupales

#### 4.7.1 Descripción

+ **Prioridad:** 3

Esta no es una función tan relevante para nuestro sistema dado que los alumnos ya tienen un gran
número de herramientas para comunicarse entre sí. Sin embargo, es importante para los proyectos
grupales y otras comunicaciones. Por esta razón, se le dio una prioridad baja.

#### 4.7.2 Estímulos / Respuestas
+ Estímulo: El alumno selecciona varios alumnos entre sus contactos para añadir al grupo.

+ Respuesta: El sistema generará el grupo e integrará a los alumnos seleccionados en caso de que estos
   aceptaren.

#### 4.7.3 Requerimientos funcionales
+ **REQ-14**: Los alumnos que sean invitados a la conversación grupal tendrán que existir en
  ConectaITAM.
  
+ **REQ-15**: Deberá existir una categoría de conversación grupal en la plataforma.

## 5 Otros requerimientos no funcionales

### 5.1 Requerimientos de rendimiento

ConectaITAM deberá mostrar el siguiente desempeño:
+ El sistema deberá actualizarse automáticamente en cuanto sea posible.
+ Cualquier solicitud deberá ser satisfecha en menos de 500ms. El desempeño dependerá de la carga en
los servidores y en la base de datos del ITAM.

### 5.2 Requerimientos de seguridad (Safety)

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

### 5.3 Requerimientos de seguridad (Security)

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

### 5.4 Atributos de calidad de software

+ **SQ-1:** El sistema será fácil de usar para todos los usuarios, se aplicará periodicamente un
sondeo a usuarios seleccionados para evaluar la calidad de diseño.

+ **SQ-2:** El sistema estará siempre disponible, con un enfoque en las horas pico. Por ello ,se
monitorearán constantemente las transacciones de datos y los incidentes que podrían llegar a
suceder.

+ **SQ-3:** El sistema contará con frecuentes copias de seguridad de los estados estables del mismo,
para que en el caso de fallas, se pueda reestablecer el servicio a los usuarios.

### 5.5 Reglas de negocio

+ **BU-1:** Solo los profesores y los administradores del sistema serán capaces de modificar los
chats grupales predefinidos.

+ **BU-2:** Solo los administradores del sistema serán capaces de bloquear permanentemente la
comunicación entre dos usuarios.

+ **BU-3:** Solo los administrativos de servicios escolares y departamentos académicos, así como los
administradores, podrán gestionar la información del chatbot.

+ **BU-4:** Los estudiantes serán capaces de bloquear, por una semana como máximo, la comunicación
con otro usuario.

# Plan de Calidad

## 1 Identificador del plan de prueba

ComunicaITAM\_1.0\_Testing\_Y4M3A8URR1

## 2 Referencias

Los documentos que respaldan este plan de calidad son:

[Plan de proyecto y requerimientos del sistema](#requerimientos-del-sistema)

## 3 Introducción

Este plan de calidad para la plataforma ConectaITAM está elaborado en torno a los más populares
navegadores _web_, tal como: Chrome, Firefox, Safari y Opera. En este documento se tiene como
objetivo:

+ Definir las herramientas para utiliar durante todo el proceso de pruebas.
+ Definir cuales son los parámetros para realizar dichas pruebas.
+ Identificar los elementos sobre los cuales se realizarán las pruebas y establecer lo que se espera
  de ellas.

Todo lo anterior se define con el fin de dar la mayor seguridad y confiabilidad a la plataforma de
comunicación ConectaITAM.

## 4 Elementos de prueba

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

## 5 Problemas de riesgo del software

Las áreas críticas del sistema ConectaITAM son:

+ Intercambio de mensajes a través de la red.
+ Almacenamiento de conversaciones, datos personales y demás información confidencial.
+ Envío de archivos multimedia.
+ Permisos de administradores, profesores y empleados administrativos.

## 6 Funcionalidades a probar

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
+ (1) Como estudiante/profesor quiero compartir un archivo multimedia.

## 7 Funcionalidades que no deben probarse

Las siguientes funciones no serán sometidas a pruebas.

+ Enviar notificaciones de nuevos mensajes.
+ Crear conversaciones grupales predefinidas.
+ Agendar una cita por medio del chatbot.

## 8 Enfoque (estrategia)

+ Se realizarán las pruebas de la siguiente manera:
  + Se tendrá una lista de funcionalidades a probar, con el resultado esperado.
  + El encargado de prueba deberá crear los escenarios de prueba para los _testers_.
  + Los _testers_ deberán reportar el resultado con aprobado, fallado u omitido.
  + Los _testers_ podrán indicar notas adicionales relevantes a las pruebas.
+ Las pruebas se realizarán de forma unitaria, en tanto se hagan disponibles las funcionalidades.
+ Cada prototipo está constituido por 2 funcionalidades del sistema, o 4 requerimientos funcionales,
  desarrollados en el orden en que se presentan en el SRS (4).
+ Adicionalmente, habrá una prueba final que consista en evaluar la plataforma como un sistema
  integrado.
+ Se utilizarán las siguientes métricas dentro de la plataforma:
  + Tipos de archivos multimedia enviados.
  + Tiempo utilizado por funcionalidad a probar.
  + Mensajes enviados por hora.
  + Utilización del chatbot.
+ Ante pruebas fallidas, se crearán _bug reports_ para su pronta atención, dependiendo de la
  severidad del problema reportado.
+ Los resultados de las pruebas se deberán discutir con el equipo una vez que los presente el
  encargado de pruebas, y con base en la prioridad de las funcionalidades, se realizarán los cambios
  pertinentes.
+ En caso de haber una falla de seguridad, se hará referencia a los riesgos de cada funcionalidad
  para determinar la prioridad de los cambios.
+ La plataforma debe probarse en Windows, MacOS y Linux, así como en los navegadores web más
  populares (Chrome, Firefox, Safari y Opera).

## 9 Criterios de aprobación/falla

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

## 10 Criterios de suspensión y requisitos de reanudación

Las pruebas para el sistema ConectaITAM deberán detenerse inmediatemente si:

+ Se experimenta error en inicio de sesión.
+ Se experimenta error en alguna acción básica como: creación, lectura, actualización y eliminación
  de solicitudes a la base de datos.
+ Existe un gran porcentaje de ciclos de prueba fallidos (más del 50% del total de los casos).
+ Incrementan notablemente el número de defectos encontrados durante las pruebas (más de 10
  defectos).

## 11 Entregables de prueba

Los entregables considerados en este plan son los siguientes:

+ Plan de prueba
+ Especificaciones del diseño de pruebas
+ Especificaciones de casos de prueba
+ Especificaciones de los procedimientos de prueba
+ *Logs* de pruebas y métricas
+ Reportes de incidentes de pruebas
+ Informes resumidos sobre las pruebas

## 12 Tareas de pruebas restantes

Para los entregables del punto anterior, se deberán cumplir las siguientes tareas:

+ Preparación del plan de pruebas.
+ Revisión y modificación, en caso de ser necesario, de los escenarios de pruebas.
+ Preparación del entorno de pruebas, de acuerdo al punto siguiente.
+ Asignación aleatoria de pruebas a los _testers_.
+ Indicación a los _testers_ de qué áreas de la plataforma se deben probar y cuáles aún no (pruebas
  unitarias parciales). En su caso, se indicará que la prueba es para toda la plataforma.
+ Recabación de datos durante y después de las pruebas, tanto de métricas como de los _testers_
  directamente. 
+ Registro de incidentes durante las pruebas al sistema.
+ Contraste con resultados esperados de cada prueba.
+ Preparación del informe de resultados de las pruebas.

## 13 Necesidades ambientales

Para llevar a cabo las pruebas, es necesario que los _testers_ cuenten con todos los sistemas
operativos y los buscadores instalados que se desean probar. Para estos, se utilizarán las versiones
más recientes únicamente. Es posible que los sistemas operativos estén instalados en máquinas
virtuales. Los resultados de las pruebas se originarán de las métricas, así como de lo indicado por
los _testers_ según el punto 8 de este documento. Las computadoras necesitarán únicamente de una
conexión de internet normal. Los _testers_, adicionalmente, requerirán de cuentas de prueba en un
entorno independiente al de producción dentro de la plataforma.

## 14 Necesidades del personal y capacitación

La capacitación del personal de pruebas deberá ser la misma que recibirán los alumnos. En caso de no
tener habilidades tecnológicas, se deberá capacitar a dichos _testers_ mediante una instrucción
razonablemente reproducible por el ITAM para sus alumnos. Todos los _testers_ recibirán el manual de
usuario que se distruibuirá a los alumnos y se les dará un tiempo razonable, pero corto, para
familiarizarse con él. Se limitará a las áreas de la plataforma relevantes a la prueba en curso. Los
_testers_ no requerirán utilizar ninguna herramienta en especial; las métricas se recaudarán
automáticamente y las notas serán escritas. El encargado de prueba deberá poder utilizar los
sistemas de reporte de incidentes, recaudación de datos y reporte de resultados.

## 15 Responsabilidades

+ El encargado de prueba será responsable de:
  + la coordinación y elaboración apropiada de todas las pruebas, en tanto sean asignadas y
  aprobadas conjuntamente con el equipo de desarrollo.
  + asegurarse que los _testers_ estén apropiadamente equipados y capacitados para realizar las
  pruebas bajo las condiciones especificadas.
  + comunicar los resultados y los incidentes durante las pruebas al equipo de desarrollo.
+ El equipo será responsable de:
  + asegurarse que el encargado reciba la capacitación relevante a la plataforma que sea necesaria
	para llevar a cabo el proceso de pruebas y la capacitación de sus _testers_.
+ Los _testers_ serán responsables de:
  + realizar las pruebas de acuerdo a las expectativas y las indicaciones que reciban.

## 16 Calendario

El periodo de implementación de las pruebas para el sistema ConectaITAM tendrán una duración de 3 semanas y se realizarán 1 mes antes de su lanzamiento. Se dividirá en tres periodos de pruebas y cada una de ellas tendrá una extensión de una semana. Cada periodo de prueba se enfocará en un bloque de funcionalidades.

| Semana | Bloque de pruebas | Usuarios objetivo |
| ------ | ------------------ | ------------------ |
|    1   | Inicio de sesión, Envíar y recibir mensajes, Creación de grupos predefinidos, Creación y gestión de chats individuales y grupales privados, Buscador de usuarios. | Estudiantes, Profesores, Administradores del sistema |
|    2   | Reporte de mensajes, reporte de ususarios, reporte de casos de acoso graves, bloqueo de usuarios, subir archivos adjuntos | Estudiantes, Profesores, Administradores del sistema, Administradores de servicios escolares |
|    3   | Principales funciones del chatbot: dar información personal del alumno, dar información general sobre dudas, agendar citas con servicios escolares | Alumnos y Administradores de servicios escolares |

## 17 Planificación de riesgos y contingencias

+ La capacitación del responsable de prueba podría probar ser más complicada de lo estimado. De ser
  el caso, la entrega del proyecto será retrasada necesariamente.
+ Es posible la revelación de algún problema grave del sistema durante las pruebas, más allá de lo
  razonablemente esperado. Esto resultaría en un retraso necesario del proyecto, dado que las fallas
  críticas son inadmisibles y sería necesario asignar tiempo para las correcciones.
+ Alguna de las funcionalidades de baja prioridad podría probar ser más compleja de lo esperado y no
  cumplir con el periodo de pruebas esperado. En este caso, el producto se entregaría de manera
  limitada, con la garantía de la entrega de la(s) funcionalidad(es) restantes en un plazo
  razonable.
+ Debido a restricciones de presupuesto, obtener el equipo suficiente para el cuerpo de pruebas
  podría ser retrasado. De ser así, el producto sería necesariamente retrasado, ya que no se puede
  continuar el desarrollo sin el ciclo de pruebas.
+ El manejo inadecuado del equipo de pruebas por parte de el encargado de prueba podría resultar en
  la insuficiencia del ciclo de prueba. Esto resultará en una degradación de la calidad del
  producto.

## 18 Aprobación

La aprobación está sujeta a que los líderes del equipo estén de acuerdo en que se han cumplido todas
las expectativas del producto, así como que la etapa de desarrollo relevante haya concluído y se
pueda continuar a la siguiente. Además, la aprobación final está sujeta a que el ITAM concuerde con
que se cumplen las políticas de la institución en todas las competencias aplicables, definidas
anteriormente en el documento de requerimientos.

# Arquitectura

ConectaITAM utiliza una arquitectura mixta entre capas y eventos. La arquitectura por eventos se utiliza en la aplicación 
al hacerse uso de un chatbot para brindar información a los alumnos.

Para la página principal se eligió la arquitectura por capas ya que consideramos que la facilidad para hacer pruebas y para 
desarollar era más benéfico que la escalabilidad u otros beneficios que ofrecen otras arquitecturas.

Consideramos que las desventajas de la arquitectua por capas son principalmente la escalabilidad y la facilidad de despliegue, pero
no creemos que nuestra aplicación vaya a recibir cambios en las reglas de negocio de manera constante. Además de esto, creemos que 
la cantidad de alumnos del ITAM se mantendrá en un rango de aproximadamente 6 mil usuarios activos.

# Metodología

La metodología que se utilizó para ConectaITAM fue de prototipos, ya que esta metodología nos permitió 
validar la esencia funcional del proyecto y realizar cambios esenciales antes de crear la solución final. 
La ventaja de esta metodología es que nos permitió recopilar los requisitos de nuestra aplicación y 
analizarla sin tener que invertir demasiados recursos.

# Casos de Uso
Caso 1: Un alumno quiere subir un documento a un grupo.
![](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/subir%20documento.PNG)

Caso 2: Un alumno crea un nuevo grupo dentro de una materia.
![](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/crear%20grupo.PNG)

Caso 3: Un alumno quiere agendar una cita con el chatbot
![](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/crear%20cita.PNG)

# Instrucciones para replicar

La liga para el proyecto se encuentra en [en esta
liga](https://jacquelinelira.github.io/ConectaItam/).

1. Para iniciar sesión se utilizan los siguientes datos: 
   + Usuario: yo 
   + Contraseña: pass 
   
2. Una vez en la pantilla de inicio, se hace _click_ sobre el texto "Aprendizaje
   de Maquina", el cual redirige al chat de ese grupo.
   
3. Al agregar un texto en el campo de texto y presionar el botón, éste aparecerá
   en la pantalla del chat. Nota: El texto que aparece es predeterminado.
   
4. Se hace _click_ en los "..." a lado izquierdo del campo de texto y se
   selecciona la opción "Subir documento".
   
5. Al pasar el ratón sobre la sección de arrastrar y soltar, se "cargan" los
   archivos arrastrados y se presiona el botón "Subir" para guardarlos en la
   plataforma.
   
6. Se hace _click_ en los "..." de nuevo y se selecciona la opción "Crear
   subgrupo".
   
7. Se llenan los campos de nombre y descripción, se seleccionan los miembros que
   se van a agregar (Gandolfo Garibay y Jorge Rosado) y se presiona el botón
   "Crear grupo"

8. Se presiona el botón del robot, el cual se encuentra en la parte superior derecha
   de la pantalla.
   
9. Se le pregunta al chatbot por la calificación de "Aprendizaje", a lo cual el
   chatbot le responde.
   
10. Se pide agendar una cita con "Becas", a lo cual el chatbot le da al usuario
   la opción de que días están disponibles (se elige la opción 1).

# Presentación

Podrá encontrar la presentación del proyecto final [aquí](https://github.com/Ingenieria-de-Software-ITAM-2020/Delfines/blob/main/presentaci%C3%B3n%20final.pdf)




