# **QA WORKFLOW**

I am Carlos Redolar, student from Videogame Design degree at [CITM Terrassa](https://www.citm.upc.edu/). This research is for Project II subject, under supervision of [Marc Garrigó](https://es.linkedin.com/in/mgarrigo).


# What is QA?

Las siglas significan "Quality Assurance", lo cual es un conjunto de acciones y actividades programadas que se realizan sobre un juego para asegurar que cumpla una série de normas, estándares y requisitos de calidad préviamente establecidos por un departamento de QA y los productores. Dicha "calidad" no siempre significa que el juego sea bueno o que vaya a agradar al público, sino que ha superado esos parámetros que el equipo y la empresa desean.

Para garantizar esta calidad se utilizan test, que ponen a prueba el juego, aunque QA engolba otros muchos procesos aparte del testing.

# QA como proceso ágil

El proceso de QA es flexible y debe adaptarse al resto de equipos, artistas, programadores... El proceso debe hacerse durante todo el proyecto, en concreto, desde que sale el primer documento de diseño podemos empezar a planificar qué y cómo lo vamos a testear.

Para poder evaluar cada milestone y cada build primero debemos definir un critério para ello, el departamento de QA y los productores debeán hacer un documento con los parámetros que cada integrante del equipo deba seguir cuando testee, además de las especifícaciones sobre cómo hacer el report.


# Diagrama de flujo

![](docs/diagram.png)


# Tipos de test según el tester

**QA Department testing:** el equipo encargado de la propia empresa porbará el juego y el código en busca de errores.

**UX testing:** el juego es probado por usuarios objetivo, a los cuales traemos expresamente para analizar sus reacciones.


# Tipos de test según la metodología

## Tests automatizados

Los tests automatizados son llevados a cabo por ordenadores de forma automática, podemos simular miles de comportamientos para así preveer o detectar posibles errores. Al ser hecho por un ordenador los procesos son muy rápidos y nos permiten ahorrar tiempo.

Las pruebas más comunes realizadas mediante este proceso son:

- **Pruebas unitarias:** hace pruebas de módulos separados de código para aislar errores. Utilizado sobretodo en core mechanics y comunicación de bases de datos.

- **Pruebas de resolución:** hace simulaciones del juego en diferentes resoluciones y simulando diferenes dispositivos para preveer el comportamiento del juego en diversos escenarios.

- **Pruebas de estrés:** se centra en simular escenarios extraños y sobrecargados para encontrar los límites del juego.


## Tests manuales

Los test manuales son llevados a cabo por personas, el lado malo de esto es que las personas son lentas y mucho menos eficientes que un ordenador, pero el factor humano nos hace capaces de encontrar errores sobre gustos y mejoras más complejas. 

Las pruebas más comunes realizadas por humanos son:

- **Pruebas de interfaz:** el equipo analiza los elementos de la interfaz, no solo que funcione correctamente sino también que sea lo más intuitiva posible.

- **Pruebas de estrés:** como hemos aclarado antes, en las pruebas de estrés intentamos poner nuestro juego al límite.

- **Pruebas de remojo:** se basa en dejar al juego haciendo una tarea pos un tiempo prolongado para ver su reacción.

- **Pruebas de sonido:** en esta prueba no solo se comprueba que los sonidos vayan, sino que también se mira que todos los audios cuadren con las animaciones o  dar feedback sobre la estética conjunta.

- **Pruebas de mecánicas:** se comprueba que las mecánicas funcionen como deberían y damos feedback sobre posibles mejoras.

- **Pruebas de humo:** es una prueba corta en la que comprobamos el correcto funcionamiento del juego sin prediseñar una prueba.

## Mix manual-automatico

Al fin y al cabo las empresas que cuentan con departamento de QA utilizan ambos metodos y se complementan, ya que el automático hecho por ordenador se dedica a tareas sencillas pero muy laboriosas en muy poco tiempo y el equipo humano de los errores que requieren más complejidad.

## Herramientas para automatizar

Para llegar a ese método mixto nos ayudamos de herramientas que nos permitan hacer el trabajo manual más fácil.
La herramienta principal de toda empresa es su propio código, creamos nuestros propios scripts que nos permitirán probar todo tipo de cosas, implementación de "godmodes", "next level", "monedas o vidas ilimitadas"...

También hay plataformas que nos proporcionan herramientas, como es el caso de Unity y su "Unity Test Tools" que nos permite hacer pruebas unitarias.


# Test Plan

La planificación del test se centra en la pregunta "Qué vamos a testear?" y "Que recursos necesitamos?". La estrategia de pruebas es un documento que detalla los procesos y maneras en que vamos a asegurar esa calidad en nuestro juego. En esta planificación definimos el proceso de pruebas, los niveles de pruebas, roles de cada miembro del equipo y cada test definido en el plan.


# Test design

El diseño de la prueba es el cómo se llevará a cabo el test y la lista de escenarios que vamos a cubrir.
Para diseñar las pruebas hay diferentes enfoques:

- **Proactivo:** son pruebas que son diseñadas lo antes posible, para preveer mas o menos dónde podemos encontrar errores incluso antes de crear la build.

- **Basado en riesgos:** son pruebas diseñadas posteriormente a la build para encontrar errores en sitios concretos.


# Report

Después de realizar cada prueba se ha de hacer un informe para informar sobre los errores e incluso los aciertos.
Las herramientas que suelen usar las empresas son: Mantis, Jira y Google Docs.

La parte más importante del report es el formato, el cual todos los miembros del equipo deben respetar para que luego le sea fácil al programador entender y resolver el error.

- **Descripción del error/bug:** breve descripción del error.

- **Estado:** estado actual del error, ya sea acabado de detectar, se esta resolviendo, esta resuelto, o no es necesario resolver.

- **Paso-paso:** descripción paso a paso de cómo llegar a que ocurra el error.

- **Comportamiento esperado:** descripción de cómo debería funcionar sin el error.

- **Relevancia:** se agrupa den 3 tipos según la importancia del bug. Tipo A para errores que afectan a la experiencia del juego. Tipo B para errores que afectan la experiencia de usuario. Y tipo C para mejoras de qualquier ámbito.

- **Prioridad:** aquí declaramos cuánto de rápido queremos solventar este error (si lo que remos arreglar), no necesariamente en el orden de relevancia, ya que puede haber errores de relevancia menor que necesitemos arreglar antes.

- **Versión:** especificamos el numero de versión o que build estamos tartando.

- **Plataforma:** especificamos en que dispositivo estamos corriendo la build en el cual hemos detectado el error.


# Sources

[https://www.youtube.com/watch?v=UF3Ya0uvYpU](https://www.youtube.com/watch?v=UF3Ya0uvYpU)

[http://www.gamerdic.es/termino/qa/](http://www.gamerdic.es/termino/qa/)

[https://apiumhub.com/es/tech-blog-barcelona/ingeniero-qa-organizando-workflow/](https://apiumhub.com/es/tech-blog-barcelona/ingeniero-qa-organizando-workflow/)

[https://usersnap.com/blog/quality-assurance-workflow/](https://usersnap.com/blog/quality-assurance-workflow/)

[https://skywell.software/blog/qa-process-flow-in-software-testing/](https://skywell.software/blog/qa-process-flow-in-software-testing/)

[https://www.softwaretestinghelp.com/what-is-actual-testing-process-in-practical-or-company-environment/](https://www.softwaretestinghelp.com/what-is-actual-testing-process-in-practical-or-company-environment/)


# Contact

email: **carlos.redolar.torres@gmail.com**



