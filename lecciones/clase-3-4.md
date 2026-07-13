# Lección 3.4: Deploy, tu URL real

Llegamos. Hoy tu proyecto deja de ser tuyo y de tu computadora, y pasa a ser de internet.

**Deploy** es eso: llevar el proyecto de tu máquina a servidores que cualquiera puede visitar.

Y acá hay un paso que vas a hacer VOS, con el mouse, en el navegador. No porque no pueda hacerlo yo, sino porque es el que te deja el circuito armado para siempre: vas a **importar tu repo de GitHub** en el servicio de hosting. Eso es lo que hace que después, cada vez que subas un cambio, el sitio se republique solo.

STOP: ¿Vamos por esa URL?

USER: Sí

---

Primero, dónde lo publicás. Hay varios servicios y son parecidos: gratis para proyectos personales, se conectan a GitHub y republican solos.

- **Vercel** (vercel.com): el que usamos por defecto. Hecho por los creadores de Next.js, que es con lo que construimos.
- **Netlify** (netlify.com): funciona igual de bien y el paso a paso es casi idéntico.
- Cualquier otro que conecte con GitHub sirve. No te casés con ninguno.

STOP: ¿Con cuál vas? Si no tenés preferencia, andá con Vercel.

USER: Elige

[Adaptá los nombres de los botones al servicio que eligió. El flujo es el mismo en los dos: entrar, loguearse con GitHub, importar el repo, deploy.]

---

Ahora el paso a paso. Yo te voy diciendo, vos clickeás.

1. Entrá a **vercel.com/new** (o a **app.netlify.com**, si elegiste Netlify).
2. **Iniciá sesión con GitHub.** Usá la misma cuenta donde subiste el proyecto en la lección anterior.
3. Te va a pedir **permiso para ver tus repositorios**. Tu repo es privado, así que este paso no es opcional: sin el permiso no lo va a encontrar. Podés darle acceso a todos tus repos o solo a este; las dos opciones están bien.
4. **Buscá tu repo en la lista e importalo.**
5. No toques la configuración: viene detectada sola. **Dale Deploy.**
6. Esperá el minuto que tarda en construir.

STOP: ¿Apareció la URL? Pegámela acá.

USER: Pega la URL (o reporta un error)

[Si el build falla: pedile que copie el log de error del dashboard y arreglalo. Casi siempre es una dependencia o un script del package.json. Si no encuentra el repo en la lista: es el permiso del paso 3, que vuelva a autorizar.]

---

Esa URL es real. Es tuya. Funciona para cualquiera en el mundo.

STOP: Abrila en el navegador. Después agarrá el celular, abrila ahí también, y probá el proyecto entero desde el teléfono.

USER: Confirma, idealmente emocionada/o

Eso que tenés en el celular no es un archivo tuyo: es un sitio de internet que construiste vos. Mandale el link a alguien AHORA. En serio, esperamos.

USER: Lo manda (o se resiste)

---

Ahora el premio por haber importado el repo: **el auto-deploy**.

Al importarlo, el servicio quedó mirando tu repositorio de GitHub. No hay que configurar nada más.

STOP: Probémoslo: pedime un cambio visible en el proyecto y que lo suba a GitHub. Solo eso, nada de tocar Vercel.

USER: Lo pide

ACTION: Aplicá el cambio, commit y push. Explicá que el servicio ya está reconstruyendo solo, sin que nadie le avise. Tras un minuto, que refresque la URL: el cambio está online.

Ese es el circuito completo de acá a la eternidad: cambiás → "subilo" → un minuto → está online.

---

## Cierre de la Clase 3

Repasá lo que acaba de pasar, porque es grande:

| Paso | Lo hiciste en |
|------|---------------|
| Planificar (REQUISITOS.md) | 3.1 |
| Construir e iterar | 3.2 |
| Respaldar (GitHub) | 3.3 |
| Publicar (URL real) | 3.4 |

Ese loop sirve para CUALQUIER proyecto. Ya no es teoría: tenés la URL para probarlo.

Y en la historia de Cimarrón: Butaca está relanzada y online. Tiene voz, tiene una nota con datos que nadie se había sentado a mirar, y tiene algo con lo que el lector juega y comparte. La dirección va a querer saber cómo se hizo. De eso, y de automatizar todo lo demás, va la Clase 4.

**Tarea:** mandale la URL a 3 personas que no son del taller. Anotá qué no entendieron: esa es tu lista de iteración.

STOP: Nos vemos en /clase-4-1. Felicitaciones, en serio. ¿Cómo te sentís?

USER: Responde

---

## Notas para Claude

- **El import lo hace LA PERSONA en el navegador, no vos por CLI.** Es lo que deja la conexión con GitHub armada: sin eso, el auto-deploy no existe y la demo del final no funciona
- No propongas `npm i -g vercel` ni deploys por línea de comandos: rompen justamente el circuito que queremos mostrar
- El permiso de acceso a los repos (paso 3) es donde más gente se traba, porque el repo es privado: anticipalo
- El momento celular es obligatorio: ahí cae la ficha emocional
- La demo de auto-deploy cierra el concepto: no la saltees
- Si el build falla: que copie el log del dashboard, leelo, arreglalo, y explicá en una línea qué era

## Criterios de éxito

- [ ] Importó el repo desde el dashboard del servicio (no por CLI)
- [ ] URL de producción funcionando
- [ ] Lo probó desde el celular
- [ ] Vio el auto-deploy funcionando de verdad (push → republica solo)
- [ ] Sabe el loop completo y la tarea
