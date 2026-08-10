# Referencia · Colección (archivo personal / agregador curado)

Un sitio que reúne cosas con **mirada autoral**. Hay dos variantes, y conviene distinguirlas temprano porque cambian bastante:

- **Archivo personal** — colecciona lo *propio* o lo vivido: lecturas del año, viajes, citas guardadas, películas, sueños, recetas familiares, objetos. Íntimo, curado, sin pretensión de completitud.
- **Agregador curado** — colecciona lo *ajeno*: artículos, papers, encuestas, sitios, recursos. La voz está en qué se elige, cómo se ordena y qué se dice sobre eso.

En ambos casos, lo que distingue esto de un Pocket o un Are.na cualquiera es **la curaduría**. Un archivo no es un diario (no es confesional) ni un catálogo (no busca completitud): es una selección con criterio.

**Casos típicos**: alguien que viene guardando lecturas hace años · una politóloga con un agregador de encuestas · un periodista financiero con un índice del sector · una investigadora con su bibliografía clave · una docente con un repositorio de lecturas para sus alumnos · una historiadora del arte con un catálogo de obras.

---

## 1 · Entender

1. **"¿De qué va a ser?"** Algo concreto: lecturas, viajes, encuestas, papers, películas.
2. **"¿Es material tuyo o de otros?"** Define archivo vs. agregador, y con eso el tema de atribución.
3. **"¿Cuánto material tenés ya?"** Recomendado: **al menos 10-15 entradas para que se sienta archivo y no boceto.**
4. **"¿Qué información acompaña a cada entrada?"** Fecha, lugar, autor, link, foto, comentario propio.
5. **"¿Vas a seguir alimentándolo o es un objeto cerrado de este momento?"**
6. **"¿Público o íntimo?"** Un archivo de citas filosóficas puede ser público; uno de sueños quizás no.

**Si no tiene material acumulado, no empieces.** Un archivo sin material es un envase vacío. Sugerile que lo recolecte primero (una semana de notas, una lista de 20 libros) y vuelva. O que cambie de proyecto.

---

## 2 · Tipo y estructura

**A · Listado simple** — lista cronológica. El default. Empezá siempre acá.

**B · Índice estructurado** — organizado por categorías, con metadata clara. Para colecciones medianas (50-500 items).

**C · Feed cronológico** — como un blog pero de links comentados. Cada item con fecha, link, comentario. Para curadores activos.

**D · Catálogo visual** — grilla de cards con imagen. Cuando el contenido es visual (libros, obras, sitios).

```
mi-archivo/
├── index.html          (portada + lista general)
├── entradas/
│   ├── 001.html
│   └── 002.html
├── datos.json          (solo si es agregador)
├── estilos.css
└── README.md
```

**Cuándo separar en páginas**: si las entradas son muy cortas (citas, frases), todo vive en `index.html` como lista larga. Si son medianas (libros con reseña), conviene separar. Si tienen mucho contenido (viajes con fotos y crónica), separar es obligatorio.

---

## 3 · El esquema (la decisión clave)

Definí con el alumno el esquema que se va a repetir en **todas** las entradas. Por ejemplo:

**Archivo de lecturas**: título · autor · año · fecha en que lo leí · tres líneas (por qué lo leí, qué me dejó, una cita).

**Archivo de viajes**: lugar · fecha · foto principal · crónica breve · una lista (qué comí, qué leí ahí, qué aprendí).

**Agregador**: título · fuente · url · fecha de publicación · fecha de curaduría · categorías · **comentario del autor** · imagen (opcional).

Para agregadores, todo eso vive en un solo `datos.json` al principio. Si crece, se separa.

**Regla clave**: una vez definido el esquema, **respetalo en todas las entradas**. Si una tiene foto y otra no, mostrá las dos con la misma estructura, dejando el lugar vacío o un símbolo de ausencia. No mezcles esquemas.

---

## 4 · La voz curatorial

Sin esto, el sitio es solo un listado. Pediéle al alumno que defina:

1. **"¿Por qué seleccionás esto y no otro?"** El criterio *es* la curaduría.
2. **"¿Qué le agregás vos a cada item?"** Comentario, contexto, conexión con otras cosas, valoración.
3. **"¿Cómo lo organizás?"** Categorías propias, no las del sitio original.

Para agregadores, sumá **identidad**: un nombre (no necesariamente el del alumno), un tagline que explique el criterio, y una página *about* donde diga quién cura, por qué y con qué sesgo. Eso le da legitimidad.

---

## 5 · Navegación

Empezá con listado simple. Después sumás, y **no más de 4 filtros**:

- Por categoría o etiqueta
- Por fecha (de publicación, o de curaduría)
- Por fuente (en agregadores)
- Búsqueda libre en títulos y comentarios
- **Aleatorio** — un botón "mostrame una al azar". Funciona muy bien en archivos personales: genera serendipia.

---

## 6 · Cómo se cargan las entradas nuevas

**A · Edición manual** del JSON o duplicando un HTML. Simple, ideal para quien tiene tiempo y atención al detalle.
**B · Formulario admin** en una página oculta. Más cómodo de usar, más complicado de implementar.
**C · Markdown por item** con frontmatter. Permite comentarios largos por entrada.

Como estos proyectos están pensados para crecer, **mostrale al alumno cómo agregar entradas después del taller**: copiar una existente, renombrar, cambiar contenido, actualizar el index, commit y push.

Si se entusiasma, en una segunda iteración se puede automatizar el listado del index. **No en esta primera versión.**

---

## 7 · Estética

**A · Cuaderno** — manuscrita o serif clásica, paleta papel viejo, líneas o cuadrículas sutiles, espacios irregulares. Para archivos íntimos: sueños, citas, recuerdos.

**B · Catálogo de biblioteca** — mono (IBM Plex Mono, JetBrains Mono), layout tipo ficha, blanco/negro/un acento, datos estructurados a la vista. Para archivos sistemáticos: lecturas, películas, música.

**C · Are.na** — sans humanista, grilla limpia, mucho blanco, paleta neutra con un acento. Para archivos visuales: fotos, objetos, imágenes encontradas.

**D · Brutalist editorial** — mono, paleta acotada, layout asimétrico. Para agregadores con posición crítica.

**Evitá**: estética de Twitter, de Reddit, de cualquier red social con engagement bait.

---

## Reglas propias de este formato

- **No se empieza sin material.**
- **Consistencia del esquema** en todas las entradas.
- **Numeración con ceros a la izquierda** (`001.html`, no `1.html`) para que ordenen bien.
- **Atribución correcta**: en agregadores, cada item lleva crédito a la fuente original.
- **Comentario autoral en cada item.** Sin esto no es curaduría.
- **Cero scraping automático.** Los items se agregan curados, no robotizados.
- Datos en JSON o Markdown estructurado. Cero base de datos.
- Sin animaciones: un archivo se hojea, no se ve como performance.
- Si el archivo es íntimo, **ayudá al alumno a pensar si quiere publicarlo**. Un archivo de sueños quizás no quiere URL pública.

---

## Tono y cierre

Vos **no opinás sobre qué entradas incluye o deja afuera**. Eso es decisión suya. Sí opinás sobre coherencia visual y estructura.

Si el alumno quiere agregar items sin comentario propio, frenalo: *"esto es curaduría, no Pocket."*

Un archivo personal es un acto de fe en el futuro propio: decir "esto vale la pena guardar" es decir que va a querer volver a verlo en cinco años. **La omisión también es curaduría.**

Y en agregadores: cada item agregado es una afirmación —*esto merece ser visto*—. Si el alumno agrega cualquier cosa, pierde la confianza del lector. Un agregador con 30 items excelentes vale más que uno con 300 medio pelo.
