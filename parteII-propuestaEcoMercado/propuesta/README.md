# Propuesta de diseño — App EcoMercado UGR

> Insights, propuesta de valor y diseño de interfaz móvil  
> Basada en el análisis de Huerta Madrid — DIU 2025/26

---

## 1. Usuarios objetivo: más allá del entorno universitario

Una de las conclusiones más interesantes del análisis de Huerta Madrid es que sus usuarios no son un perfil homogéneo. Hay gente muy habituada a comprar online y gente que necesita que todo esté explicado con mucha claridad. El EcoMercado UGR tiene exactamente el mismo reto: nace en el entorno universitario, pero su visión es abrirse para toda la ciudad.

Por eso, en lugar de crear personas nuevas, he pensado en reutilizar los dos perfiles que ya definí en el análisis de Huerta Madrid. Tienen todo el sentido aquí porque representan exactamente el rango de usuarios al que debería llegar el EcoMercado si quiere avanzar más allá del entorno universitario:

### Persona 1 — Laura, 34 años (consumidora concienciada urbana)
Laura compra online con frecuencia y sabe lo que quiere. Si llega a la app del EcoMercado UGR, espera encontrar la información rápido: cuándo es el próximo mercado, qué productores van a estar y si puede reservar algo con antelación. No tiene paciencia para procesos complicados ni para buscar información repartida por varios sitios. Si la experiencia es buena, repite; si no, no vuelve.

### Persona 2 — Marcos, 52 años (usuario ocasional poco digitalizado)
Marcos llega al EcoMercado porque alguien se lo ha recomendado o porque ha visto un cartel por la ciudad. No es un comprador online habitual y necesita que todo esté muy claro desde el primer momento: qué es esto, cuándo es, dónde es y cómo puede participar. Si la app le resulta confusa o le pide demasiados pasos, la abandona. Para Marcos, la accesibilidad y la claridad son clave.

Diseñar para estos dos perfiles a la vez es lo que va a hacer que la app sea realmente útil para todo el mundo, no solo para la comunidad universitaria.

---

## 2. Empathy Map

Sintetizo las necesidades de ambos perfiles para identificar los puntos en común que debe resolver la app:

| | Laura | Marcos |
|---|---|---|
| **¿Qué piensa y siente?** | Le parece una iniciativa genial pero le cuesta seguirle la pista si no está muy pendiente de redes sociales. | Le llama la atención pero no sabe muy bien cómo funciona ni si es para él. |
| **¿Qué ve?** | Publicaciones esporádicas en redes con poco margen de tiempo. Poca información sobre qué productores van a estar. | Un cartel por la ciudad o una recomendación de alguien. Poco más. |
| **¿Qué le duele?** | Enterarse tarde. No poder planificar qué va a comprar antes de ir. No saber si un productor concreto va a estar. | No entender el proceso. Tener miedo a llegar y no saber qué hacer. Sentir que es "para universitarios" y no para él. |
| **¿Qué gana?** | Compra de proximidad planificada, contacto con productores locales, actividades interesantes. | Una experiencia de mercado diferente, más cercana y con valores, sin complicaciones. |

La conclusión del Empathy Map es clara: los dos perfiles necesitan lo mismo, aunque por razones distintas. Información clara, accesible y a tiempo. Laura la quiere para planificarse; Marcos la necesita para no sentirse perdido.

---

## 3. ScopeCanvas — ¿Qué resuelve esta app y para quién?

Antes de ponerse a diseñar pantallas, conviene tener muy claro qué problema resuelve la app y qué no. El ScopeCanvas ayuda a delimitar eso:

| | |
|---|---|
| **Necesidades que cubre** | Saber cuándo y dónde es el próximo mercado. Conocer qué productores y productos van a estar. Reservar productos con antelación. Consultar el programa de talleres y actividades. Recibir recordatorios antes del día del mercado. |
| **Objetivos del producto** | Aumentar la asistencia al mercado más allá del entorno universitario. Reducir la incertidumbre del usuario antes de ir. Visibilizar a los productores locales. Hacer el EcoMercado accesible para cualquier persona, no solo para universitarios. |
| **Propuesta de valor** | Una app sencilla y accesible que convierte el EcoMercado UGR en una experiencia planificable para cualquier persona: sabes cuándo es, qué vas a encontrar y puedes reservar lo que quieres antes de que se agote, tanto si eres estudiante como si eres vecino del barrio. |
| **Métricas de éxito** | Asistencia por edición. Reservas realizadas. Valoración de la experiencia (SUS). Porcentaje de usuarios no universitarios. |
| **Acciones** | Poder reservar los productos de una manera fluida. Consultar información acerca de los productores. Observar los diferentes talleres y charlas que se realizan durante el evento. |

---

## 4. Arquitectura de información

### 4.1 Sitemap

La app se organiza en cuatro secciones accesibles desde la barra de navegación inferior. La estructura es sencilla y reconocible — exactamente lo que necesita un perfil como Marcos para no perderse:



### 4.2 User Flow principal — Reservar un producto

El flujo más importante de la app tiene que ser tan claro que Marcos pueda seguirlo sin ayuda la primera vez que lo usa:



Cada paso tiene una sola acción posible. No hay bifurcaciones confusas ni decisiones técnicas que el usuario no sepa tomar.

### 4.3 User Flow secundario — Inscribirse a una actividad

Al igual que el flujo anterior, con una sencilla serie de pasos una persona que no sea nativa digital podría conseguir este objetivo:



Como antes, no hay elecciones complejas, simplemente vamos directos al grano.

---

## 5. Propuesta visual — Pantallas principales

### 5.1 Identidad visual

Las decisiones de diseño visual están pensadas para transmitir los valores del EcoMercado (proximidad, sostenibilidad, confianza) sin resultar intimidantes para alguien como Marcos:

**Paleta de color:**
- Verde oscuro (`#2D6A4F`) como color principal — naturaleza y sostenibilidad sin parecer clínico
- Beige cálido (`#F4ECD8`) como fondo — evoca lo artesanal y lo orgánico, fácil de leer
- Naranja tierra (`#E07B39`) para los botones de acción — llama la atención sin ser agresivo
- Otros colores secundarios como marrón tierra (`#3A2E1A`) o el verde menta pastel (`#E8F5EE`)

**Tipografía:**
- *DM Sans* para títulos — cercana y legible
- *Inter* para cuerpo de texto — muy legible en pantallas pequeñas, sin serifs que dificulten la lectura

**Estilo general:** Limpio, cálido y sin complicaciones. Fotografía de producto y de mercado para generar confianza. Sin grandes zonas vacías — cada pantalla tiene contenido útil y justificado.

### 5.2 Pantallas principales

**Pantalla 1 — Inicio**
Lo primero que ve el usuario es la respuesta a la pregunta más urgente: ¿cuándo es el próximo mercado? Un contador grande en la parte superior, con la fecha, hora y lugar del próximo mercado bien visibles. Debajo, un acceso directo al catálogo de esta edición. Para Laura, es suficiente para planificar. Para Marcos, es suficiente para saber si puede ir.

**Pantalla 2 — Catálogo de productores**
Lista de productores con foto, nombre y una línea de descripción de qué traen. Al pulsar en uno se abre su ficha completa: quién es, de dónde viene y qué productos trae. El objetivo es que el usuario conozca a las personas detrás de los productos; algo que diferencia al EcoMercado de cualquier supermercado y que en este diseño puede funcionar al buscar ese acercamiento del campo a la mesa.

**Pantalla 3 — Ficha de producto**
Aquí está uno de los aprendizajes directos del análisis de Nuestras Huertas: la ambigüedad sobre qué se está comprando es un problema importante. En esta app, cada producto muestra de forma clara y explícita la foto real del producto, el nombre, el productor, la unidad de venta (ej. "bolsa de 500g", "docena de huevos", "1 kg"), el precio y la disponibilidad. Sin lugar a confusión.

**Pantalla 4 — Actividades**
Los talleres y charlas son una parte importante del EcoMercado que en la mayoría de webs de referencia queda en segundo plano. Aquí tienen su propia sección, con hora, descripción breve y opción de apuntarse. Para Laura es un valor añadido; para Marcos puede ser la razón por la que decida ir.

**Pantalla 5 — Mis reservas**
Resumen claro de lo que el usuario ha reservado para el próximo mercado. Puede modificar o cancelar antes del día del mercado. El día anterior llega una notificación de recordatorio con el resumen del pedido. Simple, sin sorpresas.

### 5.3 Accesibilidad desde el principio

A diferencia de lo que encontré en Nuestras Huertas, aquí la accesibilidad se planifica desde el inicio:

- Buen uso del contraste en todos los textos (nivel AA de WCAG 2.1)  
- Áreas táctiles suficientes en todos los botones y enlaces
- Texto alternativo descriptivo en todas las imágenes
- Navegación sencilla sin menús anidados ni opciones confusas

---

*Los wireframes de las pantallas descritas están disponibles en la carpeta [`wireframes/`](./wireframes/).*

---

*Alejandro Gea Martínez · DIU · Curso 2025/26 · Universidad de Granada, ETSIIT*
