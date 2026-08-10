# Referencia · Pieza autoral (fanzine, bestiario, experimental)

Una pieza web con voz propia, donde **la estética es contenido** y se pueden romper convenciones a propósito. No es un sitio funcional ni una herramienta: es el formato más libre del taller. No tiene función comercial, no tiene público que servir, no rinde cuentas.

**Casos típicos**: una diseñadora que quiere un fichero tipográfico con personalidad · una artista visual que muestra una serie · un periodista que quiere un dossier con voz propia · una activista con una pieza-manifiesto · alguien que quiere hacer un fanzine, un bestiario, un tributo.

---

## 1 · Entender la intención autoral

Antes de lo técnico, entender qué quiere expresar:

1. **"¿Qué querés que el visitante *sienta* al entrar?"** No qué información dar. Qué sentir.
2. **"¿Hay alguna pieza, libro, fanzine, sitio que te inspire?"** Si tiene referencias, son oro.
3. **"¿Cuál es el tono?"** Melancólico, lúdico, irónico, rabioso, contemplativo, urgente, íntimo, místico, paródico.
4. **"¿Hay una sola idea fuerte o varias?"** Las mejores piezas autorales suelen ser monotemáticas.
5. **"¿El visitante interactúa o solo contempla?"**

Si el alumno no puede responder, **no avances con código**. Las piezas experimentales sin intención clara salen vacías.

---

## 2 · Elegir la sub-forma

### Fanzine

Publicación autogestionada, hecha por amor o por urgencia, sin filtro editorial. Tipografías mezcladas, composición intuitiva, fotocopia, collage, contrastes altos. **No vende: declara.**

El riesgo: hacer "una web limpia con onda zine". Eso no es un fanzine, es una landing con texturas. Un fanzine digital tiene que arriesgar visualmente. Tiene que ser un objeto, no una página.

Componentes: **tapa** (título, número, año, autoría) · **editorial** (por qué este fanzine, por qué ahora) · **páginas o secciones** (textos, manifiestos, listas, poemas, collages) · **colofón** (créditos, contacto, agradecimientos).

Navegación: scroll único (más fácil en celular) · paginado tipo libro con anterior/siguiente (más fiel al impreso) · no lineal con índice.

### Bestiario

Catálogo medieval de criaturas con descripción, ilustración y significado. El formato se reapropió: hoy cualquier cosa puede tratarse como "criatura". Borges en *Manual de zoología fantástica*, Cortázar en *Bestiario*. Hay bestiarios del capitalismo, de la oficina, de objetos domésticos.

Lo importante: **un bestiario es un catálogo con un punto de vista.**

Cada entrada lleva: **nombre** (con o sin latín falso, según el tono) · **símbolo o imagen** · **descripción** (3-5 líneas) · **hábitat** · **atributos** (3-5 items) · **anotación del bestiarista** (una línea con voz propia, irónica o melancólica). El alumno puede sumar campos (peligrosidad, dieta, relación con humanos) o sacar.

Arrancá con 5-10 criaturas. El index es **portada, no listado plano**: un bestiario tiene umbral, ritual de entrada.

### Otras formas

**Manifiesto** — una sola pantalla, una idea grande, mucha presencia tipográfica.
**Pieza-experiencia** — el sitio mismo es la experiencia. Click, scroll, hover: todo significa.
**Tributo** — dedicado a alguien o algo. Cercano al ensayo personal.
**Generador** — produce algo distinto cada vez (frases, imágenes, combinaciones).

```
mi-pieza/
├── index.html          (la tapa / portada / umbral)
├── paginas/            (o criaturas/, o entradas/)
│   ├── 01.html
│   └── ...
├── estilos.css         (donde vive toda la locura visual)
└── README.md
```

---

## 3 · El manifiesto estético (obligatorio)

Acá es donde este formato se diferencia de todos los demás. **No empieces a construir sin esto:**

1. **Una palabra que defina la estética**: brutalist, naïf, melancólica, glitchy, austera, barroca, retro-90s, punk, post-internet.
2. **Una pieza de referencia**: un sitio, un libro, un cuadro, un disco con esa estética. Pedísela al alumno.
3. **Tres reglas claras**:
   - Qué **siempre** va a estar (tipografía X, color Y, gesto Z).
   - Qué **nunca** va a estar.
   - Qué convención rompemos **a propósito**.

Sin manifiesto, la pieza sale genérica.

---

## 4 · Estética

**A · Punk fotocopia** — tipografías mezcladas (una serif clásica con una deforme), texturas de papel, alto contraste, blanco y negro con un acento estridente (rojo sangre, amarillo flúor, verde lima). Asimetrías intencionales.

**B · Brutalismo digital** — mono o sans condensada, fondos planos, bordes gruesos, sin imágenes o con imágenes pixeladas. Títulos enormes, párrafos angostos, vacíos largos.

**C · Riso print / neoexpresionismo** — paleta de 2-3 colores planos (rosa + azul + negro), sans humanista, ilustraciones geométricas simples, todo "imperfecto" a propósito.

**D · Manuscrito iluminado** — fondo crema, serif (Cormorant Garamond), capitulares grandes, ornamentos discretos. Sobrio, antiguo. Ideal para bestiarios.

**Tipografías arriesgadas de Google Fonts**: Redaction, Tiny5, VT323, Major Mono Display, Pilowlava, IBM Plex Mono, Space Grotesk, DM Serif Display.

**Comprometete con la elección.** Un fanzine tibio es peor que un fanzine fallido. Si dice "lo quiero brutalist", que sea brutalist en serio. Si dice "melancólico", que duela mirarlo. La timidez estética es lo único que arruina estas piezas.

---

## 5 · Imágenes

**A · Propias del alumno** — lo ideal. Da identidad genuina.
**B · CSS art** — formas con CSS puro. Estética muy específica pero coherente.
**C · SVG inline** — vectores escritos en el HTML. Permite personajes, símbolos custom.
**D · Ninguna** — la tipografía y el espacio hacen todo el trabajo.

**Evitá**: stock photos, imágenes de IA pegadas sin contexto, capturas random.

**Detalles que suman**: sombra de pliegue o marcas de fotocopiado con `box-shadow` inset suave · imágenes tratadas con `filter: grayscale()`, `contrast()`, `sepia()` · cursor que cambia sobre los links.

---

## 6 · Validar la voz

Cada tanto, preguntale al alumno:

- "¿Esto suena como vos?"
- "¿Lo subirías a tu Instagram?"
- "¿Lo defenderías frente a tus amigos?"

Si la respuesta es dudosa, ajustá. Estas piezas se notan cuando se hacen sin convicción.

---

## Reglas propias de este formato

- **No avances sin manifiesto estético** (punto 3).
- **Animaciones bienvenidas si suman al gesto.** Acá sí puede ser más expresivo que en otros formatos — pero con criterio.
- **Cero placeholder, sin excepción.** Una pieza autoral sin contenido real no es una pieza. Si el alumno no tiene el texto, paramos hasta que lo escriba.
- **Sin emojis** en el contenido salvo pedido explícito. Mejor SVG inline para símbolos.
- **Mobile-first con ojo**: el impreso tiene formato fijo; en digital hay que adaptarse a pantallas chicas sin perder el carácter. Discutilo con el alumno.
- El README acá es breve: título, un párrafo sobre qué es y por qué existe, créditos.

---

## Referencias mencionables

- Borges, *Manual de zoología fantástica* / *El libro de los seres imaginarios* · Cortázar, *Bestiario* (1951)
- Bestiarios medievales: Aberdeen Bestiary, Rochester Bestiary
- Zines argentinos: La Cebolla, Sudaka, La Cosa
- Riso print: Risolab BA, Hato Press
- Collages punk: Jamie Reid (Sex Pistols), Linder Sterling
- Are.na, buscando "fanzine", "zine" o "bestiary"

---

## Tono y cierre

Como **un editor con un autor**: respeto a las decisiones autorales, pero capacidad de cuestionarlas.

- Si el alumno propone algo genérico: *"esto se siente AI slop, ¿lo querés más arriesgado?"*
- Si propone algo demasiado pulido: *"esto te queda muy limpio para fanzine, ¿lo ensuciamos un poco?"*
- Si propone algo ilegible: *"esto es muy fanzine, pero no se entiende. Bajemos un poco."*
- Si tiene una idea arriesgada que vos no entendés: **no la frenes.**

Estas piezas tienen un valor que las comerciales no: **son evidencia de que la persona tuvo algo para decir**. Si la pieza del alumno podría existir tal cual en un blog corporativo, algo está mal. Si es lo que es porque *solo podría* ser esto, vamos bien.

No tiene que ser entendida por todos. Tiene que ser **suya**. Eso alcanza.
