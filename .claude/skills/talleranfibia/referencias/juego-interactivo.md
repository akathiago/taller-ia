# Referencia · Juego interactivo

Un mini-juego web con HTML, CSS y JavaScript. Nada de Unity, ni Phaser, ni motores. Solo código vainilla, pero hecho con criterio y diversión.

**Casos típicos**: una docente que quiere un juego sobre cambio climático para adolescentes · una diseñadora que rediseña un juego de mesa clásico · un periodista con una trivia política para su audiencia · una creativa con un generador aleatorio · alguien que vio el dino de Chrome y quiere su versión.

---

## 1 · Tipo de juego

**A · Trivia o quiz** — preguntas con respuestas múltiples, puntaje al final.
**B · Memotest** — pares de cartas, encontrar parejas. Puede ser temático.
**C · Generador aleatorio** — click y sale algo al azar. Frases, combinaciones, decisiones imposibles.
**D · "Qué tipo de X sos"** — quiz tipo BuzzFeed, 5 preguntas, resultado personalizado.
**E · Plataformero simple** — estilo dino de Chrome. Un personaje, obstáculos, score creciente.
**F · Click-to-collect** — click en cosas que aparecen, sumar puntos, tiempo limitado.
**G · Puzzle** — sokoban, sliding puzzle, wordle, alguna mecánica de razonamiento.
**H · Aventura conversacional** — texto que avanza con decisiones, bifurcaciones, múltiples finales.

Cada categoría tiene su complejidad. A, B, C y D son las más accesibles para alguien que recién empieza.

---

## 2 · El tema

Un juego es memorable cuando tiene tema. No es lo mismo "trivia de cultura general" que "trivia de literatura argentina del siglo XX".

1. "¿Qué tema te apasiona o sabés mucho?"
2. "¿A quién le querés mostrar este juego?"
3. "¿Querés que sea sobre algo que ya sabés o sobre algo que quieras aprender?"

Sin tema claro, el juego sale genérico.

---

## 3 · Alcance realista (el paso que más se saltea)

La trampa más común: querer hacer un juego más grande de lo posible. Dividí con el alumno:

- **Lo mínimo viable** — la mecánica básica, una pantalla, un loop completo. **Esto se construye primero, siempre.**
- **Lo que estaría bueno** — score, animaciones, sonidos.
- **Lo que es lujo** — niveles, multijugador, persistencia.

**No avances sin definir el mínimo viable.**

---

## 4 · Estructura

```
mi-juego/
├── index.html      ← estructura
├── estilos.css     ← apariencia
├── juego.js        ← lógica
└── README.md       ← cómo se juega
```

Si crece, separá la lógica: `estado.js` (variables y estado) · `render.js` (lo que dibuja) · `eventos.js` (teclado, mouse).

### Decisiones técnicas por tipo

- **Trivia / memotest / quiz** → JS puro, datos en JSON, manipulación del DOM. Simple.
- **Con animación** (plataformero, click-to-collect) → `requestAnimationFrame` para el game loop. Posiciones con CSS transforms o canvas.
- **Pixelado** → `<canvas>` con `image-rendering: pixelated`.
- **Con sonido** → HTML5 Audio API. Pocos sonidos, bien elegidos.
- **Generadores** → `Math.random()`. Sin complicaciones.

---

## 5 · Los visuales

**Claude no genera imágenes.** Las opciones son:

**A · CSS puro** — personajes y elementos con divs estilizados. Estética naïf, minimalista, indie. **Recomendá esta salvo que el alumno sea diseñador o tenga preferencia clara.**
**B · SVG inline** — formas vectoriales por código. Más sofisticado, más esfuerzo.
**C · Emojis** — rápido y reconocible, aunque se ven distinto en cada sistema operativo.
**D · Sprites descargados** — de Kenney.nl o similar. Mejor estética, requiere preparación previa.

---

## 6 · Estética

**A · Pixel art / 8-bit** — pixelado, paleta limitada, fuente mono. Arcade clásico.
**B · Editorial minimalista** — tipografía elegante, paleta sobria, sin decoración. Juego "de autor".
**C · Brutalist / experimental** — tipografías grandes, paletas agresivas, layouts no convencionales. Para juegos-arte.

---

## 7 · UX

- **Instrucciones claras al principio.** Si el jugador no sabe cómo jugar en 5 segundos, perdiste.
- **Feedback inmediato**: cada acción tiene una reacción visible.
- **Estado siempre visible**: score, vidas, tiempo.
- **Reinicio fácil**: volver a jugar sin recargar la página.
- **Controles táctiles** que funcionen, si aplica.

---

## 8 · El "feel"

Estos detalles chicos son la diferencia entre un juego "ok" y uno memorable:

- Transiciones suaves entre estados.
- Pequeñas animaciones en hover y click.
- Sonidos minimalistas (un beep al click, una nota al ganar).
- Vibración corta **del elemento** (no de la pantalla) cuando algo falla.
- **Mensajes con personalidad**: "¡La rompiste!", "Otra vez será", "Casi casi".

---

## Reglas propias de este formato

- **Sin frameworks ni motores de juego.**
- **Una sola página** salvo justificación clara.
- **El juego tiene que ser jugable después de cada iteración.** No dejes versiones rotas.
- **Cero sprites de IA pegados sin contexto.** CSS, SVG o sprites descargados con licencia clara.
- **Performance**: si el game loop va trabado, simplificá.
- **Nunca avances sin definir el alcance mínimo viable.**
- Acá **sí** van animaciones: son parte del juego.
- El README lleva: cómo se juega · controles · objetivo · créditos.

---

## Tono y cierre

**Lúdico y energético.** Estás haciendo un juego, no un Excel. Celebrá los hitos: la primera vez que se ve el personaje, la primera vez que se mueve, la primera victoria.

Si el alumno se entusiasma con features grandes, validalo pero traelo al mínimo viable primero. Si se traba con la mecánica, simplificá.

Los juegos web no compiten con AAA. **Tienen que dar gracia, sorprender y divertir dos minutos.** Eso alcanza. Un buen juego web es como una buena tarjeta de cumpleaños: chiquito, hecho con cariño, memorable. No el próximo Fortnite: algo que un amigo abra, juegue dos minutos y sonría.

Si el juego es pieza pedagógica (caso típico: docentes), recordale que **el aprendizaje viene del juego repetido**, no del contenido del juego. Que diseñe una mecánica que invite a jugar varias veces, no a leer cinco preguntas y listo.
