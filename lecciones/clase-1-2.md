# Lección 1.2: Ver y referenciar archivos

Hasta ahora trabajaste a ciegas: yo te cuento qué hay en los archivos y vos me creés. Eso se termina hoy.

Vamos a armar tu espacio de trabajo visual: yo de un lado, tus archivos del otro, los dos a la vista. Vas a VER los archivos aparecer y cambiar mientras trabajo.

STOP: ¿Tenés instalado VS Code u Obsidian? Si no tenés ninguno, decime y vemos opciones.

USER: Responde

[Si tiene VS Code o Obsidian: guialo para abrir la carpeta del taller ahí (VS Code: File → Open Folder). Si no tiene nada: recomendale instalar VS Code de code.visualstudio.com, acompañalo, y mientras baja podés seguir con la parte del @; también sirve el Explorador de Windows como plan B temporal.]

---

Antes de seguir, una pregunta que me ahorra hacerte perder tiempo después.

STOP: ¿Desde dónde me estás hablando ahora mismo? Tres opciones: (1) la **terminal** (la pantalla negra donde escribiste `claude`), (2) el **panel de Claude adentro de VS Code** (el que se abre con el ícono de la chispa), o (3) la **app de escritorio de Claude**. Cualquiera vale, solo necesito saber cuál.

USER: Responde

[Anotá la respuesta: la vas a necesitar toda la clase. Los tres caminos completan el taller, pero los gestos cambian (ver la tabla de superficies en SCRIPT_INSTRUCTIONS.md). Si está en la terminal, decile que eligió el camino donde todo funciona igual que en los apuntes. Si está en el panel o en Desktop, tranquilizala/o: se hace todo igual, cambian un par de botones y te los voy indicando. En la lección 1.4 esto queda anotado en la memoria del proyecto y no se pregunta nunca más.]

---

Ahora acomodemos el espacio para que me veas trabajar. Cómo se arma depende de dónde estés:

[Dale SOLO la versión de su superficie:

- **Terminal:** acomodá las ventanas, la terminal de un lado y VS Code (o el editor que uses) del otro. Pantalla partida, las dos visibles al mismo tiempo.
- **Panel de VS Code:** buena noticia, ya lo tenés armado: yo vivo en la barra lateral y tus archivos están al lado. Lo único: abrí el explorador de archivos (el ícono de las hojitas, arriba a la izquierda) para ver la carpeta entera mientras trabajamos.
- **App de escritorio:** yo estoy en mi ventana y tus archivos en la suya. Abrí VS Code (o el Explorador de Windows / Finder) en la carpeta del taller y ponelo al lado mío, así ves los archivos cambiar en vivo.]

STOP: ¿Ves los archivos de la carpeta del taller y me ves a mí, los dos al mismo tiempo?

USER: Sí

[Si no ve los archivos: seguramente abrió otra carpeta. Decile la ruta exacta de la carpeta actual y que abra exactamente esa.]

Perfecto. Ahora mirá el editor mientras yo hago algo.

ACTION: Creá un archivo prueba-visual.md con un saludo personalizado (usá su nombre) y una línea que diga que este archivo se creó mientras miraba.

STOP: ¿Lo viste aparecer? Abrilo en el editor y leelo.

USER: Confirma

Eso es trabajar con visibilidad. Nunca más "¿qué habrá hecho?". Ahora borrémoslo para no dejar basura.

ACTION: Borrá prueba-visual.md y confirmá que lo hiciste.

---

Segunda parte de la lección: el símbolo más importante de todos.

`@` es la forma de señalarme archivos. `@archivo.md` es "mirá este archivo". `@carpeta/` es "mirá toda esta carpeta". Cuando empezás a escribir @, te sugiero los archivos disponibles: elegís con las flechas y Tab.

Probemos con el desastre que te dejaron.

STOP: Pedime que lea @caos-heredado/notas-del-editor-anterior.md y te diga en qué estado están esas notas.

USER: Lo pide referenciando el archivo con @

ACTION: Leé las notas y resumí el caos con gracia: pendientes vencidos, ideas sueltas, la frase de la directora ("correcta pero no mueve"). NO menciones todavía la idea del test/quiz: guardala para la lección 2.1, donde es el descubrimiento central. Si la persona la menciona porque la vio, seguile la corriente con un "anotala, eh, puede valer oro", sin desarrollarla.

STOP: Ahí tuviste tu primera probada del caos. ¿Notaste que las notas mencionan una carpeta de comentarios de lectores que nadie leyó? Eso lo atacamos en la Clase 2, y te adelanto que ahí está enterrado el diagnóstico. ¿Todo claro con el @ hasta acá?

USER: Sí

---

Última cosa: la carpeta oculta `.claude/`. Ahí viven los comandos del taller (como /clase-1-1) y otras cosas que vamos a tocar en la Clase 4. El Explorador de Windows la esconde por defecto (Vista → Elementos ocultos para verla). VS Code la muestra siempre. Por ahora solo tenés que saber que existe.

## Cierre

Lo que te llevás:

1. **Los archivos siempre a la vista**, sea con pantalla partida o con el editor al lado. Trabajar a ciegas es opcional y es peor.
2. **@ es señalar**: archivos y carpetas, con autocompletado
3. **Los archivos aparecen en tiempo real** mientras trabajo

STOP: ¿Seguimos? /clase-1-3 te espera con los comandos y el botón de pánico.

USER: Sí / /clase-1-3

---

## Notas para Claude

- El archivo de prueba se crea Y se borra de verdad
- NO spoilear la idea del quiz de las notas del editor: es el descubrimiento de la 2.1
- Si usa Obsidian: recordale que .claude/ no se ve ahí, y que use el Explorador para eso

## Criterios de éxito

- [ ] Tiene los archivos y a Claude a la vista al mismo tiempo (el arreglo que corresponda a su superficie)
- [ ] Vio un archivo crearse en tiempo real
- [ ] Usó @ para referenciar un archivo
- [ ] Leyó (resumidas) las notas del editor anterior
- [ ] Sabe que .claude/ existe y está oculta
