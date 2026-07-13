# Lección 3.1: Planificar tu proyecto

Arranca la Clase 3. Al final de esta clase hay una URL real con algo construido por vos. Hoy: la planificación.

Primero, el nombre de lo que vamos a hacer: **vibecoding**. Construir software describiendo lo que querés. Vos no vas a programar: vas a dirigir. Tu laburo es saber qué querés, dar buen feedback y darte cuenta cuándo está bien. El código es problema mío.

---

Lo que vamos a construir es **Butaca**: la sección relanzada, como sitio de verdad. Tres piezas, y cada una contesta algo del diagnóstico que hiciste en la Clase 2:

1. **La portada.** Butaca no tenía identidad: era "correcta pero olvidable". La portada es donde eso se arregla: nombre, voz, actitud. Que se note de quién es apenas entrás.
2. **La nota.** El editor anterior dejó una nota a medio escribir sobre los datos del INCAA (@caos-heredado/notas-a-medio-escribir/nota-incaa-sin-terminar.md) y nunca la terminó. La terminás vos, con los datos de @caos-heredado/estrenos-incaa.csv. Es la prueba de que Butaca sí puede contar la industria sin aburrir.
3. **El quiz.** "¿Qué clásico del cine argentino sos?" La pieza que hace lo único que Butaca nunca hizo: que el lector participe y comparta.

Informar, sí. Pero además: tener voz y hacer participar. Eso es la sección entera, no un test suelto.

STOP: ¿Construimos el sitio de Butaca o tenés un proyecto propio que preferís hacer con el mismo proceso? Los dos caminos valen, y el proceso es idéntico.

USER: Elige

[Si elige proyecto propio: mismo guion, adaptando la entrevista a su idea. Buscá igual que tenga tres piezas o menos: una identidad, un contenido y algo interactivo. Esa estructura es la que hace que el proyecto se pueda terminar hoy.]

---

Todo proyecto sigue el mismo loop: **planificar → construir → iterar → guardar → publicar**. Hoy hacemos la primera parte, que es la que la gente saltea y después llora.

Los requisitos son el contrato: qué hace la cosa, cómo se ve, qué pasa en cada interacción. Instrucciones vagas dan resultados inesperados. Así que te voy a entrevistar.

STOP: Pedime que te entreviste para definir los requisitos del sitio, y que al final guarde todo en REQUISITOS.md.

USER: Lo pide

ACTION: Entrevistala/o de a UNA pregunta por vez, en tres bloques. No apures.

**Bloque 1 — la portada (rápido, 2 preguntas):** (1) ¿qué es lo primero que ve el lector al entrar, y qué tiene que sentir? (2) ¿qué promete Butaca en una frase? (esa frase va a ser el título de la portada; que salga de la persona, con el tono de contexto/VOZ-DE-CIMARRON.md).

**Bloque 2 — la nota (rápido, 2 preguntas):** (1) ¿cuál es el título? (el borrador propone "El cine argentino no está muerto (los datos)": validalo o mejoralo con la persona) (2) ¿qué tiene que entender el lector que NO entendía antes? Anotá que la nota se escribe con los datos reales del CSV, sin inventar cifras, y que el borrador del editor ya tiene la tesis: se estrenan más películas argentinas que nunca y las ve menos gente que nunca.

**Bloque 3 — el quiz (el más largo, es el corazón):** (1) ¿cuántas preguntas? (sugerí 6-8), (2) ¿qué resultados posibles? (sugerí 4 clásicos del cine argentino bien distintos entre sí, definilos con la persona; que sean películas reales), (3) ¿qué tono tienen las preguntas? (con humor, estilo Cimarrón), (4) ¿qué muestra el resultado? (descripción con gracia + por qué te tocó + botón de compartir). Explicá en el camino la LÓGICA: cada respuesta suma puntos para un resultado, gana el que más tiene. Eso es todo el "algoritmo", y lo acaba de diseñar la persona, no vos.

STOP: [Al terminar la entrevista] ¿Algo que quieras agregar o cambiar antes de que congele los requisitos?

USER: Confirma o ajusta

ACTION: Creá REQUISITOS.md completo, con una sección por pieza: portada (título, promesa, qué se ve), nota (título, tesis, qué datos del CSV se usan), quiz (contenido completo de preguntas y resultados escritos con el tono de la revista, y el mapa de puntajes respuesta → resultado). Agregá una sección de estilo visual, pendiente de los previews. Y una última sección: **orden de construcción** (quiz → portada → nota), que es como lo vamos a levantar mañana.

---

Falta lo visual, y acá va un truco de oro: nunca describas estética con palabras. "Moderno" no significa nada. Se PIDE VER.

STOP: Pedime 3 previews HTML de la portada de Butaca con estilos bien distintos (por ejemplo: editorial sobrio, retro de cine de barrio, lúdico colorido), abiertos en el navegador.

USER: Lo pide

ACTION: Generá 3 archivos preview-1.html, preview-2.html, preview-3.html con la portada en tres estéticas bien diferenciadas, y abrilos. Que se vean el título, la promesa y los accesos a la nota y al quiz: son las tres piezas.

STOP: ¿Cuál va? Podés mezclar ("la tipografía del 1 con los colores del 3"). Esta decisión define el look de TODO el sitio, no solo de la portada.

USER: Elige

ACTION: Registrá la decisión visual en REQUISITOS.md y borrá los previews que no van (o movelos a ordenado/ si la persona quiere guardarlos).

---

## Cierre

Tenés un contrato: REQUISITOS.md con las tres piezas, la lógica del quiz, el contenido y el estilo decididos por vos. En la próxima lección, yo construyo y vos dirigís.

Dato para tu vida profesional: esta entrevista de requisitos sirve igual con diseñadores, agencias o desarrolladores humanos. Acabás de aprender a especificar, que es una habilidad más valiosa que programar.

STOP: ¿Vamos a construir? /clase-3-2

USER: Sí / /clase-3-2

---

## Notas para Claude

- La entrevista es de a UNA pregunta por vez, sin apurar. Portada y nota son rápidas; el quiz es donde se pone el tiempo
- El contenido del quiz (preguntas y resultados) se escribe COMPLETO en REQUISITOS.md, con el tono de VOZ-DE-CIMARRON.md
- Los resultados son películas argentinas reales elegidas con la persona; el texto de cada resultado es descriptivo y con humor, sin inventar datos fácticos de las películas
- La nota usa los datos de estrenos-incaa.csv y NADA más: cero cifras inventadas (LEEME-DATOS.md aclara que son datos de práctica)
- Los previews se generan y se abren de verdad
- Si la persona se entusiasma y quiere seis secciones más: frenala con cariño. Tres piezas publicadas hoy valen más que diez a medio hacer

## Criterios de éxito

- [ ] Eligió proyecto (sitio de Butaca o propio)
- [ ] Pasó por la entrevista de las tres piezas y definió la lógica de puntajes del quiz
- [ ] Existe REQUISITOS.md completo, con orden de construcción
- [ ] Eligió estilo visual desde previews reales
