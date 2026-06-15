# Análisis UX: nuestrashuertas.com

> Evaluación heurística, accesibilidad, responsive y experiencia de usuario  
> Referente de análisis para la propuesta EcoMercado UGR 

---

## 1. ¿A quién va dirigida esta web? Definición de usuarios

Antes de entrar a valorar la interfaz, lo primero es preguntarse quién la va a usar. Si no tienes claro eso, cualquier análisis se convierte en una opinión personal. Aplicando la metodología de **Personas** (DCU, Tema 3), identifico dos perfiles que me parecen representativos de los usuarios de Huerta Madrid:

### Persona 1 — Consumidor urbano concienciado
- **Nombre:** Laura, 34 años
- **Perfil:** Vive en Madrid, compra online con frecuencia y le importa la alimentación ecológica y sostenible.
- **Objetivo:** Suscribirse a una cesta semanal de verdura sin complicaciones, igual que haría en cualquier otra tienda online.
- **Frustración principal:** Procesos de compra que se salen de lo esperado o que requieren pasos manuales innecesarios.

### Persona 2 — Usuario ocasional poco digitalizado
- **Nombre:** Marcos, 52 años
- **Perfil:** No es un comprador online habitual. Llega a la web por recomendación de alguien y quiere informarse antes de decidirse.
- **Objetivo:** Entender qué ofrece la web, qué productos tienen y cómo puede comprar o visitar el mercado físico.
- **Frustración principal:** Navegación confusa o procesos que asumen conocimientos técnicos que él no tiene.

Estos dos perfiles son importantes porque revelan que la web tiene que funcionar bien para usuarios muy distintos: alguien que espera una experiencia de ecommerce estándar y alguien que necesita que todo esté explicado con claridad.

---

## 2. Evaluación heurística (Nielsen, 1994)

Aplico las **10 heurísticas de Nielsen** con una escala de severidad del 0 al 4 (0 = sin problema, 4 = problema crítico que bloquea al usuario).

| # | Heurística | Observación | Severidad |
|---|---|---|---|
| 1 | Visibilidad del estado del sistema | No hay indicadores de progreso ni confirmaciones claras durante el proceso de compra. El usuario no sabe en qué punto está. | 3 |
| 2 | Coincidencia con el mundo real | El lenguaje es cercano y natural, lo cual está bien. Sin embargo, en la tienda online no queda claro si estás comprando una pieza, un kilo o una bolsa de cada producto, algo crítico en una tienda de alimentación. [→ Ver captura](capturas/04_tienda_unidades_confusas.png) | 3 |
| 3 | Control y libertad del usuario | La vía de compra por Excel, aunque está rota (ver heurística 5), plantea un flujo en el que el usuario tiene muy poco control una vez enviado el pedido por email. La tienda online sí permite modificar el carrito. | 2 |
| 4 | Consistencia y estándares | El diseño visual es bastante consistente en general. Sin embargo, algunas imágenes de producto no se corresponden con lo que se vende: por ejemplo, las cajas de fruta de temporada de distintos tamaños comparten exactamente la misma foto, lo que genera desconfianza. [→ Ver captura](capturas/05_cajas_fruta_misma_foto.png) | 2 |
| 5 | Prevención de errores | **Problema crítico:** el enlace al proceso de compra por Excel lleva a una página de error (404 — página no encontrada). El usuario que intenta comprar por esa vía queda bloqueado sin ningún aviso previo. [→ Ver captura](capturas/03_error_404_excel.png) | 4 |
| 6 | Reconocimiento antes que recuerdo | El proceso de compra por Excel requiere que el usuario recuerde rellenar un archivo y enviarlo por correo, lo que supone una carga de memoria totalmente fuera de lo habitual. La tienda online mejora esto, pero sigue sin dejar claro qué unidad se está comprando en cada producto.  [→ Ver captura](capturas/04_tienda_unidades_confusas.png) | 3 |
| 7 | Flexibilidad y eficiencia de uso | No hay atajos ni funciones avanzadas para usuarios expertos. La web funciona de la misma manera para todos. | 1 |
| 8 | Estética y diseño minimalista | Visualmente la web es agradable, pero en escritorio el layout de ancho fijo deja grandes márgenes laterales vacíos que hacen que el contenido parezca flotando en el centro. No es un problema grave, pero sí reduce la percepción de calidad. [→ Ver captura](capturas/01_home_escritorio_margenes.png)| 2 |
| 9 | Ayuda a reconocer y recuperarse de errores | El error 404 del enlace roto no ofrece ninguna alternativa ni explicación. El usuario simplemente ve "página no encontrada" y no sabe qué hacer a continuación. [→ Ver captura](capturas/03_error_404_excel.png) | 4 |
| 10 | Ayuda y documentación | Existe una sección "Cómo comprar" con bastante información, aunque el proceso que describe (Excel + email) resulta difícil y puede confundir más que ayudar a alguien que espera una compra online normal. [→ Ver captura](capturas/06_como_comprar.png)| 2 |

**Problemas más graves:**
- 🔴 Enlace roto (404) en el flujo de compra por Excel — viola heurísticas 5 y 9
- 🔴 Falta de información sobre unidades de producto en la tienda online — viola heurísticas 2 y 6
- 🟠 Imágenes de producto que no se corresponden con lo vendido — viola heurística 4
- 🟠 Ausencia de feedback durante la interacción — viola heurística 1

---

## 3. Usability Review

Usando el checklist de usabilidad visto en clase, la puntuación global queda así:

| Categoría | Puntuación |
|---|---|
| Navegación y arquitectura de información | 7/10 |
| Diseño visual y consistencia | 6/10 |
| Proceso de compra / flujo principal | 3/10 |
| Feedback y prevención de errores | 2/10 |
| Accesibilidad | 5/10 |
| Adaptación móvil (responsive) | 4/10 |
| **TOTAL** | **45/100** |

Una puntuación de **45/100** está bastante por debajo del umbral aceptable de 70/100. El proceso de compra arrastra la nota hacia abajo por dos razones: el enlace roto que bloquea una de las dos vías de compra, y la confusión en la tienda online sobre qué se está comprando exactamente (unidades, pesos, formatos). Aunque la tienda online funciona, la experiencia de selección de productos no es lo suficientemente clara como para considerarla bien resuelta.

---

## 4. Análisis de accesibilidad (WCAG 2.1)

Reviso los cuatro principios **POUR** de las pautas WCAG 2.1 (W3C, 2018):

### Perceptible
- Algunos textos en verde claro sobre fondo blanco no presenta un buen contraste exigido para nivel AA.
- Algunas imágenes carecen de texto alternativo descriptivo, lo que perjudica a usuarios que usan lectores de pantalla.

### Operable
- La navegación por teclado no está completamente resuelta, algunos menús desplegables no responden correctamente al uso del tabulador y el enter.
- En móvil, varios botones y enlaces tienen áreas táctiles bastante pequeñas que dificultan el uso.

### Comprensible
- El contenido textual es claro y el lenguaje está bien adaptado al público objetivo.
- Sin embargo, el proceso de compra por Excel rompe completamente con el patrón esperado por un usuario acostumbrado al comercio electrónico, lo que lo hace bastante confuso para la mayoría.

### Robusto
- La web funciona en los principales navegadores modernos.
- El enlace roto (404) es el punto más débil en términos de robustez: un flujo principal que no funciona es un fallo difícil de justificar.

**Conclusión:** La web no alcanza el nivel AA de WCAG 2.1 en varios criterios, especialmente en contraste de color y operabilidad por teclado.

---

## 5. Análisis responsive (escritorio vs. móvil)

| Aspecto | Escritorio | Móvil |
|---|---|---|
| Layout | Ancho fijo centrado, grandes márgenes vacíos a los lados | Contenido sin márgenes laterales que fomenta sensación de agobio  [→ Ver captura](capturas/02_home_movil_agobio.jpg) |
| Navegación | Menú horizontal accesible | Menú hamburguesa funcional |
| Imágenes | Bien dimensionadas | Se escalan correctamente |
| Proceso de compra | Enlace Excel roto (404), pero tienda online disponible y funcional | Tienda online funcional y razonablemente usable |
| Tipografía | Legible, tamaños adecuados | Correcta en general |
| Espaciado | Excesivo en los laterales | Insuficiente, sin respiración lateral |

Lo que más llama la atención del responsive es que la web parece diseñada con un ancho fijo en mente, sin pensar realmente en cómo se va a ver en pantallas grandes ni en pantallas pequeñas. En escritorio el contenido queda flotando en el centro con demasiado espacio vacío a los lados, lo que da una sensación extraña de que falta contenido. En móvil el problema es el contrario: el contenido colapsa hasta los bordes sin dejar margen para respirar. Un diseño verdaderamente responsive debería resolver ambos contextos de forma óptima, no sacrificar uno para no complicar el otro.

---

## 6. Síntesis: lo que funciona y lo que no

### ✅ Lo que funciona
- Identidad visual agradable y coherente con los valores del proyecto
- Lenguaje cercano y auténtico que conecta bien con el público objetivo
- Contenido informativo rico sobre productos, filosofía y mercados
- La tienda online ofrece una alternativa de compra más estándar que el proceso por Excel

### ❌ Lo que no funciona
- Enlace roto (404) que bloquea el flujo de compra por Excel — problema crítico
- Proceso de compra por Excel completamente fuera de los estándares actuales
- Falta de información sobre unidades de producto en la tienda online
- Imágenes que no se corresponden con el producto real
- Diseño responsive mal resuelto en ambos extremos (escritorio y móvil)
- Deficiencias de accesibilidad en contraste y navegación por teclado

---

## 7. Insights para el EcoMercado UGR

Del análisis anterior saco cinco conclusiones que van a guiar la propuesta de diseño:

1. **El flujo de consulta e información tiene que ser inmediato.** El usuario del EcoMercado llega con una pregunta concreta: ¿cuándo es el próximo mercado y dónde? Eso tiene que estar visible sin necesidad de buscar.
2. **El diseño tiene que ser mobile-first.** El público universitario consulta todo desde el móvil. No se puede diseñar para escritorio y adaptar después.
3. **Si hay información sobre productos, tiene que ser clara y sin ambigüedad.** Unidades, precios, productores — todo visible y sin lugar a confusión.
4. **La identidad visual tiene que transmitir proximidad y sostenibilidad** sin caer en el espacio vacío que aporta una sensación de no ser una web "muy trabajada".
5. **La accesibilidad tiene que planificarse desde el principio**, no como un parche posterior.

---

*Alejandro Gea Martínez · DIU · Curso 2025/26 · Universidad de Granada, ETSIIT*
