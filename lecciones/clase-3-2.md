# Lección 3.2: Construir e iterar

Hay contrato (REQUISITOS.md). Hoy se construye.

Dos conceptos rápidos antes, para que nada te suene a magia negra:

1. **Servidor de desarrollo:** un programa que corre en tu compu y te muestra el proyecto como página web mientras lo armamos. Solo lo ves vos.
2. **localhost:3000:** la dirección de ese ensayo privado. NO es una URL real: no se puede compartir. La URL real llega en la lección 3.4.

Y una regla de método, que es la que hace que hoy termines con algo publicable: **construimos por capas.** Primero el quiz, que es el corazón. Después la portada, que lo envuelve. Después la nota. Cada capa queda funcionando antes de arrancar la siguiente, así en cualquier momento tenés algo que se puede mostrar. Nadie se queda con las tres cosas a medias.

STOP: ¿Listo/a? Activá el modo Plan: para una construcción grande, conviene que veas el plan antes de que toque nada. (Gesto según tu superficie: Shift+Tab en la terminal, o el selector de modo si estás en el panel o en Desktop.)

USER: Activa el modo Plan

STOP: Ahora pedime que construya el sitio según @REQUISITOS.md, **empezando por el quiz**, y que cuando esté listo lo levante en el navegador.

USER: Lo pide

ACTION: En modo Plan, presentá el plan en castellano claro: las tres piezas, en qué orden, qué pantallas tiene cada una. Cuando lo apruebe, construí **solo la capa 1: el quiz completo y funcionando** (Next.js, que es lo que después va derecho a Vercel). Levantá el servidor y abrí localhost. Si falta Node.js, guiá la instalación desde nodejs.org con paciencia.

STOP: Ahí está el quiz, funcionando. Jugalo entero una vez y volvé. ¿Qué tal?

USER: Lo prueba y comenta

---

Ahora la parte más importante de la lección: **iterar no es arreglar errores, es EL método.** La primera versión nunca es la final, ni acá ni en ningún equipo profesional. La diferencia es que conmigo cada vuelta tarda segundos.

STOP: Decime tres cosas que cambiarías del quiz. Las que sean: tamaño, colores, textos, comportamiento.

USER: Pide cambios

ACTION: Aplicá los cambios de a uno, mostrando el resultado tras cada uno, para que sienta el ritmo del ciclo.

---

Y el truco estrella para iterar: la captura marcada.

STOP: Sacale una captura al quiz, marcá algo con un círculo o flecha (con Paint alcanza), pegala acá con Ctrl+V y decime qué querés distinto en eso que marcaste.

USER: Pega captura con marca

ACTION: Aplicá el cambio señalado. Remarcá el aprendizaje: señalar con imagen es más preciso que describir con palabras.

---

## Capa 2: la portada

El quiz está. Ahora lo envolvemos: Butaca necesita una casa.

STOP: Pedime la portada según @REQUISITOS.md, con el estilo que elegiste en los previews, y que el quiz quede enlazado desde ahí.

USER: Lo pide

ACTION: Construí la portada con la identidad definida (título, promesa, voz de Cimarrón) y el acceso al quiz funcionando. Mostrala en el navegador. Que se vea que ya no es "una página cualquiera": tiene nombre y tiene actitud.

STOP: Entrá a la portada y de ahí al quiz, como haría un lector. ¿Se siente una sección de verdad?

USER: Confirma

---

## Capa 3: la nota que nadie terminó

Última pieza, y es la más linda: la nota que el editor anterior dejó por la mitad.

STOP: Pedime que termine la nota usando el borrador (@caos-heredado/notas-a-medio-escribir/nota-incaa-sin-terminar.md), los datos de @caos-heredado/estrenos-incaa.csv, y que la publique como sección del sitio.

USER: Lo pide

ACTION: Escribí la nota de verdad: la tesis del borrador (se estrenan más películas argentinas que nunca y las ve menos gente que nunca) verificada contra el CSV, con las cifras reales del archivo y CERO cifras inventadas. Si los datos contradicen la intuición del editor, decilo: eso también es la nota. Sumá una visualización simple de la caída de la cuota de pantalla si el tiempo da. Publicala como sección del sitio, enlazada desde la portada.

STOP: Leela completa. Esa nota estuvo un año a medio escribir en una carpeta, y la terminaste vos con datos. ¿Cómo quedó?

USER: Responde

---

## Si algo se rompe (va a pasar, es normal)

La regla de oro: **los errores no se interpretan, se copian.** Texto rojo en la terminal → me lo pegás tal cual. Página en blanco → F12 en el navegador, pestaña Console, y me pegás lo rojo. Yo los leo, vos no tenés por qué.

STOP: ¿El sitio está en un punto que te gusta? No hace falta perfecto: hace falta mostrable. Lo seguís puliendo cuando quieras.

USER: Confirma

---

## Cierre

Construiste un sitio real dirigiendo, no programando: una sección con voz propia, una nota con datos y una pieza interactiva. Está viva en tu máquina. Falta que exista para el resto del mundo: eso son las próximas dos lecciones (respaldo y publicación).

STOP: ¿Vamos? /clase-3-3

USER: Sí / /clase-3-3

---

## Notas para Claude

- El modo Plan se usa de verdad: plan visible, aprobación, construcción
- **Las capas son sagradas: el quiz funciona ANTES de empezar la portada, y la portada ANTES de la nota.** Si el tiempo se corta, se corta la última capa y el proyecto igual se publica. Nunca dejes tres piezas a medio hacer
- El servidor queda corriendo; explicá que Ctrl+C lo apaga
- Los tres cambios + la captura marcada son el corazón pedagógico: no los saltees
- En la nota: ninguna cifra que no esté en el CSV. Si falta un dato, se dice que falta
- Ante errores de entorno (Node, puertos), resolvé con calma y en castellano

## Criterios de éxito

- [ ] El quiz corre en localhost y se juega entero
- [ ] Existe la portada con identidad, y el quiz enlazado desde ahí
- [ ] La nota está terminada con datos reales del CSV (o quedó explícitamente pendiente, con el sitio igual publicable)
- [ ] Entendió servidor local vs URL real
- [ ] Iteró al menos 3 cambios + 1 con captura marcada
- [ ] Sabe qué hacer con los mensajes de error (copiarlos, no interpretarlos)
