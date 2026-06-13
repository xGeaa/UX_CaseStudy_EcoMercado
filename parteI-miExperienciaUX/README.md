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

Llevándolo a lo que estudiamos en el Tema 2 (el factor humano), este fallo me pareció de libro. El conductor no era torpe; el problema es que su modelo mental estaba automatizado tras décadas usando semáforos normales (rojo = parar, verde = avanzar). Al meter un sistema nuevo sin avisar, el diseño rompió sus esquemas — lo que Norman (2013) llamaría una ruptura de la affordance esperada y un fallo de consistencia con el sistema previo. Mi propuesta de mejora fue clara: cuando cambias un código visual tan interiorizado, necesitas acompañarlo de campañas de información.

La metodología de observación (el esquema Who/What/Where...) me vino genial para aprender a separar lo que pasa de verdad de mis propias suposiciones, algo básico en UX Research para no contaminar los datos con sesgos.

**Lo mejor:** Elegir un problema real, local y muy actual.

**A mejorar:** Me faltó haber podido entrevistar al conductor en el momento; habría sumado muchísima información cualitativa.

---

## 2. Prácticas: Case Study UX — Al Burguers (basado en Goiko)

El grueso de la asignatura ha sido el rediseño de la web de Goiko para crear nuestra propia propuesta: Al Burguers. Más que listar las tareas que hicimos, prefiero centrarme en los golpes de realidad que me llevé en cada fase.

### De la investigación al insight (P1)

Como programador, mi tendencia natural siempre ha sido saltarme la teoría e ir directo a la solución técnica. El análisis de la competencia (Competitive Analysis) me obligó a frenar. Comparar Goiko con otras webs me demostró que una interfaz muy atractiva visualmente puede ser un desastre en usabilidad: menús ocultos, sin buscador, jerarquías caóticas... Al aplicar las heurísticas de Nielsen, empecé a ver los fallos con números y datos objetivos, no con opiniones.

Crear a las Personas (Martín y Sofía) me ayudó a quitarme el sesgo de "diseñar para mí mismo". Yo habría hecho la web pensando en un usuario joven y tecnológico, pero ellos tenían frustraciones y contextos totalmente distintos. Ver sus bajones emocionales en los Journey Maps me dejó claro que la experiencia de usuario es un proceso con baches, y que ahí es justo donde hay que rascar para mejorar. Cerramos con un Usability Review de 72/100; una nota que me hizo ver que la evaluación heurística es rápida y útil, aunque me quedé con la espinita de saber qué habría opinado un usuario real.

### Del análisis al diseño (P2)

En la P2 nos dimos cuenta de que el verdadero problema de Goiko no era la estética, sino la accesibilidad de los alérgenos. Las tablas de intolerancias eran infumables y densas. Ese fue el insight que definió nuestro valor diferencial para Al Burguers.

Aterrizar esto en decisiones reales fue un reto. El ScopeCanvas nos ayudó a no intentar abarcar todo de golpe, y los User Flows me abrieron los ojos: diseñar algo tan "tonto" como reservar una mesa implica mapear un montón de caminos, errores del usuario y respuestas del sistema. Cuando pasamos los primeros wireframes a Figma, por fin sentí que el proceso tenía sentido y que no estaba improvisando las pantallas sobre la marcha.

### El moodboard y la identidad visual: más difícil de lo que parece (P3)

Antes de llegar al prototipo final, tuvimos que pasar por una fase que me resultó sorprendentemente complicada: el moodboard y la definición de la identidad visual. En teoría suena sencillo — elige unos colores y una tipografía — pero en la práctica es todo lo contrario.

Al ponerte a buscar tipografías te das cuenta de que existen literalmente miles de opciones. Google Fonts solo ya tiene más de mil familias tipográficas. El reto no es encontrar una que "quede bien", sino elegir una que transmita exactamente lo que quieres: cercanía, profesionalidad, modernidad, calidez... y que además sea legible en pantalla a distintos tamaños. Con los colores ocurre exactamente lo mismo: la teoría del color te da las herramientas, pero aplicarlas a un proyecto concreto requiere muchas pruebas y descartes. ¿Qué tono de verde transmite frescura sin parecer clínico? ¿Qué marrón evoca a los ingredientes sin resultar anticuado? Hay decisiones que parecen menores pero que definen completamente la percepción que un usuario tiene del producto antes de leer una sola palabra.

Esta experiencia me enseñó que la identidad visual no es decoración: es comunicación. Y que detrás de cada decisión estética bien hecha hay un razonamiento que la justifica.

### El prototipo y la evaluación (P3, P4 y P5)

El momento clave fue terminar el Layout HI-FI. Ver todo integrado en Figma (homepage, carta, eventos) con sus transiciones y animaciones me hizo encajar todas las piezas del puzle.

Ya no elegía una tipografía (como Cabin) o un color (como el marrón cálido) porque "quedaban bien", sino porque respondían a una estrategia: transmitir cercanía y asociarse al producto. El Atomic Design fue clave aquí; trabajar desde los átomos hasta los organismos me enseñó que si quieres un diseño escalable, tienes que planificarlo como si fuera una rueda que poco a poco va acelerando hasta que al final todo es más rápido.

Terminamos en la P5 evaluando el diseño con un cuestionario SUS. Aunque los usuarios eran del todo adecuados, me sirvió para entender cómo medir la experiencia de forma estandarizada. Además, evaluar el Caso B de otro grupo me obligó a ponerme las gafas de crítico y analizar el trabajo ajeno con objetividad.

Una de las técnicas que más me llamó la atención durante las prácticas fue el uso de mapas de calor para evaluar el diseño. Creamos tres usuarios y simulamos cómo cada uno de ellos recorrería visualmente las diferentes páginas de Al Burguers, obteniendo como resultado mapas de calor que mostraban las zonas de mayor y menor atención.  

Lo que más sorprende de esta técnica es lo que revela sobre la diferencia entre cómo el diseñador cree que el usuario va a mirar su interfaz y cómo la mira realmente. Hay elementos en los que pones mucho esfuerzo de diseño que el usuario simplemente ignora, y otros que concentran toda la atención sin que lo hayas planificado así. Eso tiene consecuencias directas: si una llamada a la acción clave cae fuera de las zonas calientes, es invisible para el usuario aunque esté perfectamente diseñada.  

Aplicarlo a nuestras propias pantallas fue especialmente útil porque nos obligó a validar decisiones que hasta ese momento habíamos tomado de forma intuitiva: si la jerarquía visual que habíamos construido en Figma se correspondía con la jerarquía visual que un usuario real percibiría. En algunos casos coincidía, en otros no tanto, y esas discrepancias son exactamente el tipo de insight que guía las iteraciones del diseño. Es una herramienta que convierte algo tan difícil de medir como la atención visual en datos concretos y objetivos.  
  
---

## 4. Experiencia personal: Ricota, una webapp de rol rediseñada desde cero

Poco antes de comenzar esta asignatura, estuve programando por mi cuenta **Ricota**, una app en React, Vite y Firebase para gestionar fichas de personajes de Pathfinder 2e.

El proyecto lo empecé al revés de como he aprendido en clase: me centré en la arquitectura de datos y la base de datos. ¿El resultado? La app funcionaba por detrás, pero la interfaz era horrible. Formularios infinitos, textos apelotonados y una carga cognitiva brutal para cualquiera que entrase por primera vez. Como no sabía cómo arreglarlo, le pedí a una IA generativa que me hiciera el diseño visual. Quedó más vistoso, sí, pero seguía siendo incómodo de usar porque el problema no era de colores, sino de estructura.

A mitad de curso empecé a encajar conceptos. La arquitectura de información me hizo ver por qué el usuario se perdía. Las heurísticas de Nielsen me dieron las palabras exactas para definir los errores: falta de feedback, nulas opciones para corregir fallos y consistencia cero entre pantallas.

La consecuencia directa es que he llegado a la conclusión de que voy a tirar el frontend por completo y rehacer Ricota desde cero con metodología DCU. Antes de tocar código, voy a definir las personas (jugadores novatos vs. veteranos), mapear los flujos clave (crear ficha, actualizar datos en mitad de una partida) y prototipar en Figma. Además, pienso aplicar el sistema de componentes atómicos que aprendí con Al Burguers para crear un Design System propio. Este va a ser mi verdadero caso de estudio, y esta vez con usuarios reales (mi grupo de juego).

---

## 5. Autovaloración

Esta asignatura me ha cambiado el chip como informático. He pasado de pensar el software desde "dentro" (la base de datos, el código) a pensarlo desde "fuera" (el usuario).

**Mis puntos fuertes:** Sé cómo planificar una investigación de usuarios (User Research Plan), aplicar el checklist de Nielsen sin fallar y estructurar un diseño escalable con componentes atómicos. También he desarrollado una capacidad crítica que antes no tenía: puedo analizar una interfaz ajena e identificar sus problemas con criterios objetivos, no con opiniones. Eso es algo que ya aplico en mi día a día cuando uso aplicaciones o webs, y que antes simplemente no hacía.

Otro punto fuerte ha sido aprender a trabajar con un proceso iterativo. En programación estoy acostumbrado a pensar en soluciones definitivas; en UX he aprendido que el diseño es siempre un trabajo en progreso, que se afina con cada ronda de feedback y que equivocarse pronto y con poco coste es parte del método, no un error.

**Mis puntos débiles:** Me falta experiencia evaluando con usuarios de carne y hueso. He tirado mucho de personas ficticias, y aunque son útiles para estructurar el pensamiento, no sustituyen la riqueza de observar a un usuario real enfrentarse a tu diseño sin ninguna guía. También me queda por profundizar en accesibilidad: aunque vimos las pautas WCAG 2.1 en los seminarios, reconozco que en nuestro prototipo final pasamos un poco de puntillas. No revisamos el contraste de color con herramientas específicas ni comprobamos la navegabilidad por teclado por ejemplo, que son aspectos básicos en cualquier diseño profesional.

Ambas carencias las tengo presentes de cara al análisis del EcoMercado UGR: precisamente pretendo aplicar allí una evaluación de accesibilidad más rigurosa y proponer un diseño que tenga en intente tener en cuenta perfiles de usuario reales y diversos, cerrando así el ciclo entre lo aprendido en clase y su aplicación a un caso concreto.

---


*Alejandro Gea Martínez — DIU — Curso 2025/26*
*Universidad de Granada, ETSITT*
