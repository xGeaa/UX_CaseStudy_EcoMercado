# Parte I: Mi Experiencia UX

> Portfolio personal de interfaces, usabilidad y experiencia de usuario — DIU 2025/26

---

## Introducción

Para ser sincero, cuando empecé esta asignatura mi perfil era el de un programador puro: sabía montar la lógica de una app, pero de diseño de interfaces e investigación con usuarios no tenía ni idea. Pensaba que el diseño era algo puramente estético y subjetivo.

Este curso me ha servido para romper ese mito. He aprendido que un buen diseño no va de que la pantalla quede "bonita", sino de seguir una metodología clara, basarse en datos y, sobre todo, tener empatía con la persona que va a usar lo que programas. A continuación, resumo lo que ha sido mi proceso de aprendizaje a lo largo de las prácticas.

---

## 1. Actividad de Etnografía: El semáforo bicolor de Granada

Para la primera actividad decidí observar un caso real que me pillaba muy de cerca: el cruce de Calle Arabial con Calle Méndez Núñez, aquí en Granada. El Ayuntamiento acababa de implantar un sistema de semáforos bicolor donde el rojo y el amarillo se encienden a la vez para avisar de que va a cambiar a verde.

Durante mi observación, vi cómo un conductor aceleró antes de tiempo porque interpretó esa mezcla de colores como un "ya puedes pasar", lo que casi provoca un accidente.

Llevándolo a lo que estudiamos en el Tema 2 (el factor humano), este fallo me pareció de libro. El conductor no era torpe; el problema es que su modelo mental estaba automatizado tras décadas usando semáforos normales (rojo = parar, verde = avanzar). Al meter un sistema nuevo sin avisar, el diseño rompió sus esquemas — lo que Norman (2013) llamaría una ruptura de la *affordance* esperada y un fallo de consistencia con el sistema previo. Mi propuesta de mejora fue clara: cuando cambias un código visual tan interiorizado, necesitas acompañarlo de campañas de información.

La metodología de observación (el esquema Who/What/Where...) me vino genial para aprender a separar lo que pasa de verdad de mis propias suposiciones, algo básico en UX Research para no contaminar los datos con sesgos.

**Lo mejor:** Elegir un problema real, local y muy actual.

**A mejorar:** Me faltó haber podido entrevistar al conductor en el momento; habría sumado muchísima información cualitativa.

---

## 2. Prácticas: Case Study UX — Al Burguers (basado en Goiko)

El grueso de la asignatura ha sido el rediseño de la web de Goiko para crear nuestra propia propuesta: **Al Burguers**. Más que listar las tareas que hicimos, prefiero centrarme en los golpes de realidad que me llevé en cada fase.

### De la investigación al insight (P1)

Como programador, mi tendencia natural siempre ha sido saltarme la teoría e ir directo a la solución técnica. El análisis de la competencia (*Competitive Analysis*) me obligó a frenar. Comparar Goiko con otras webs me demostró que una interfaz muy atractiva visualmente puede ser un desastre en usabilidad: menús ocultos, sin buscador, jerarquías caóticas... Al aplicar las heurísticas de Nielsen, empecé a ver los fallos con números y datos objetivos, no con opiniones.

Crear a las Personas (Martín y Sofía) me ayudó a quitarme el sesgo de "diseñar para mí mismo". Yo habría hecho la web pensando en un usuario joven y tecnológico, pero ellos tenían frustraciones y contextos totalmente distintos. Ver sus bajones emocionales en los Journey Maps me dejó claro que la experiencia de usuario es un proceso con baches, y que ahí es justo donde hay que rascar para mejorar. Cerramos con un Usability Review de 72/100; una nota que me hizo ver que la evaluación heurística es rápida y útil, aunque me quedé con la espinita de saber qué habría opinado un usuario real.

### Del análisis al diseño (P2)

En la P2 nos dimos cuenta de que el verdadero problema de Goiko no era la estética, sino la accesibilidad de los alérgenos. Las tablas de intolerancias eran infumables y densas. Ese fue el *insight* que definió nuestro valor diferencial para Al Burguers.

Aterrizar esto en decisiones reales fue un reto. El ScopeCanvas nos ayudó a no intentar abarcar todo de golpe, y los User Flows me abrieron los ojos: diseñar algo tan "tonto" como reservar una mesa implica mapear un montón de caminos, errores del usuario y respuestas del sistema. Cuando pasamos los primeros wireframes a Figma, por fin sentí que el proceso tenía sentido y que no estaba improvisando las pantallas sobre la marcha.

### El prototipo y la evaluación (P3 y P4)

El momento clave fue terminar el Layout HI-FI en la P3. Ver todo integrado en Figma (homepage, carta, eventos) con sus transiciones y animaciones me hizo encajar todas las piezas del puzle.

Ya no elegía una tipografía (*Cabin*) o un color (marrón cálido) porque "quedaban bien", sino porque respondían a una estrategia: transmitir cercanía y asociarse al producto. El Atomic Design fue clave aquí; trabajar desde los átomos (botones) hasta los organismos me enseñó que si quieres un diseño escalable, tienes que planificarlo como si fuera código limpio.

Terminamos en la P4 evaluando el diseño con un cuestionario SUS. Aunque los usuarios eran ficticios, me sirvió para entender cómo medir la experiencia de forma estandarizada. Además, evaluar el Caso B de otro grupo me obligó a ponerme las gafas de crítico y analizar el trabajo ajeno con objetividad.

---

## 3. Experiencia personal: Ricota, una webapp de rol rediseñada desde cero

Mientras hacía la asignatura, estuve programando por mi cuenta **Ricota**, una app en React, Vite y Firebase para gestionar fichas de personajes de Pathfinder 2e.

El proyecto lo empecé al revés de como he aprendido en clase: me centré en la arquitectura de datos y la base de datos. ¿El resultado? La app funcionaba por detrás, pero la interfaz era horrible. Formularios infinitos, textos apelotonados y una carga visual brutal para cualquiera que entrase por primera vez. Como no sabía cómo arreglarlo, le pedí a una IA generativa que me hiciera el diseño visual. Quedó más vistoso, sí, pero seguía siendo incómodo de usar porque el problema no era de colores, sino de estructura.

A mitad de curso empecé a encajar conceptos. La arquitectura de información (Sem DIU07) me hizo ver por qué el usuario se perdía. Las heurísticas de Nielsen me dieron las palabras exactas para definir los errores: falta de feedback, nulas opciones para corregir fallos y consistencia cero entre pantallas.

La consecuencia directa es que voy a tirar el frontend y rehacer el proyecto completamente desde cero con metodología DCU. Antes de tocar código, voy a definir las personas (jugadores novatos vs. veteranos), mapear los flujos clave (crear ficha, actualizar datos en mitad de una partida) y prototipar en Figma. Además, pienso en aplicar el sistema de componentes atómicos que aprendí con Al Burguers para crear un Design System propio. Este va a ser mi verdadero caso de estudio, y esta vez con usuarios reales (la gente con la que juego).

---

## 4. Autovaloración

Esta asignatura me ha cambiado el chip como informático. He pasado de pensar el software desde "dentro" (la base de datos, el código) a pensarlo desde "fuera" (el usuario).

**Mis puntos fuertes:** Sé cómo planificar una investigación de usuarios (User Research Plan), aplicar el checklist de Nielsen fácilmente y estructurar un diseño escalable con componentes atómicos.

**Mis puntos débiles:** Me falta experiencia evaluando con usuarios de carne y hueso (solo he utilizado personas ficticias) y profundizar en accesibilidad. Aunque vimos las pautas WCAG 2.1 en los seminarios, reconozco que en nuestro diseño final de prácticas pasamos un poco por encima sobre esto.

Ambas carencias las tengo presentes de cara al análisis del EcoMercado UGR: precisamente pretendo aplicar allí una evaluación de accesibilidad más rigurosa y proponer un diseño que tenga en cuenta perfiles de usuario más reales y diversos, cerrando así el ciclo entre lo aprendido en clase y su aplicación a un caso concreto.

---

*Alejandro Gea Martínez — DIU — Curso 2025/26*
*Universidad de Granada, ETSIIT*
