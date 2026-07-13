# Lección 4.2: Automatizar tu rutina

La pregunta que ordena esta lección: **¿qué hacés todas las semanas que es siempre igual?**

STOP: Contestala en serio. ¿Cuál es TU tarea repetitiva más odiada?

USER: La cuenta

[Guardá su respuesta: el final de la lección es automatizar ESO.]

---

Primero lo hacemos con la rutina de Butaca, para aprender el mecanismo. En la Clase 2 armaste un resumen de prensa a mano. Hoy lo convertimos en **skill**.

Una skill es una carpeta con un archivo adentro: `.claude/skills/prensa/SKILL.md`. Arriba lleva una descripción de para qué sirve, y abajo, tus instrucciones. Nada más que texto. Los /clase-X-Y de este taller son primos hermanos de esto (andá a espiarlos cuando quieras).

STOP: Pedime que cree una skill "prensa" que busque noticias de cine argentino de las últimas 24hs, arme el resumen con el formato de @plantillas/resumen-prensa.md y lo guarde en ordenado/ con la fecha del día.

USER: Lo pide

ACTION: Creá `.claude/skills/prensa/SKILL.md` de verdad: frontmatter con una `description` bien escrita (que diga cuándo usar la skill: "cuando la persona pide el resumen de prensa de cine, las noticias del día o la ronda de medios") y, abajo, las instrucciones completas: qué buscar, en qué formato, dónde guardarlo, y la cláusula anti-verso ("si no hay noticias relevantes, decirlo sin inventar"). Mostrá el archivo abierto y explicá las dos partes: la descripción es para que YO sepa cuándo usarla; el cuerpo es lo que hago cuando la uso. Avisá que hay que reiniciar Claude Code para que la levante.

STOP: Mirá el archivo. Es texto plano: tu proceso, documentado y ejecutable. Reiniciá Claude Code y volvé.

USER: Reinicia

---

Ahora el momento lindo. No me pidas la skill por su nombre. **Pedime la tarea como se la pedirías a un colega.**

STOP: Decime algo tipo "necesito el resumen de prensa de hoy", con tus palabras, sin nombrar ninguna skill ni ningún comando.

USER: Lo pide con palabras normales

ACTION: Dejá que la skill se dispare sola (por la descripción) y ejecutala completa. Cuando termine, señalá lo que pasó: la persona no se acordó de ningún comando ni de ningún nombre, pidió la tarea como se la pediría a alguien, y el proceso salió tal cual lo definió ella.

Eso es lo que las hace distintas de un atajo: **no tenés que acordarte de que existen.** (Igual podés invocarla a mano escribiendo `/prensa`, si preferís. Y si alguna vez ves un archivo suelto en `.claude/commands/`, es lo mismo en versión mínima: un comando es una skill sin carpeta y sin descripción.)

STOP: ¿Se entiende el mecanismo?

USER: Sí

---

Ahora la receta general, la que te llevás para siempre:

1. **Hacé la tarea a mano conmigo una vez**, prestando atención
2. Cuando salió bien: **"convertí exactamente esto en una skill"**
3. **Usala una semana**, ajustá el archivo con lo que falte
4. Resultado: tu proceso, documentado, y que se dispara cuando lo necesitás

Y la regla de seguridad: **no automatices lo que no entendés.** Primero a mano, después skill.

---

Ahora sí: tu tarea odiada, la de la primera pregunta.

STOP: Hagámosla a mano una vez, ahora. Explicame la tarea con el detalle que le explicarías a alguien nuevo en tu trabajo, y la hacemos juntos (con datos de ejemplo si no tenés los reales acá).

USER: La explica y la hacen

ACTION: Ejecutá la tarea con lo que haya disponible (datos de ejemplo si hace falta). Cuando el resultado esté aprobado, proponé el paso 2 de la receta.

STOP: ¿Salió como querías? Entonces pedímelo: "convertí exactamente esto en una skill".

USER: Lo pide

ACTION: Creá la skill de SU tarea en `.claude/skills/<nombre>/SKILL.md`, con una `description` que describa bien cuándo dispararla (usá las palabras que USA LA PERSONA para nombrar esa tarea, no las tuyas: es lo que hace que se active sola cuando la pida naturalmente) y el cuerpo con los pasos, el formato de salida y dónde guardar. Si la tarea necesitara conectarse con apps externas (mail, Notion, Drive), mencioná que eso existe y se llama MCP: es el escalón siguiente, se configura una vez, y puede pedírmelo cuando lo necesite.

STOP: Última cosa y cerramos: guardá una copia de esta skill en `~/.claude/skills/` (la carpeta tuya, no la del taller). Ahí vive en TODOS tus proyectos, no solo en este. Pedímelo y lo hago.

USER: Lo pide

ACTION: Copiá la skill a la carpeta personal (~/.claude/skills/) y explicá la diferencia en una línea: la del proyecto viaja con el proyecto y se comparte con quien lo tenga; la personal es tuya y te sigue a todas partes.

---

## Cierre

Te llevás dos skills: la de prensa (de Butaca) y la tuya, la de tu vida real, que ya vive en tu carpeta personal y te va a seguir a cualquier proyecto. Y la receta para fabricar todas las que quieras.

La próxima lección es la última del taller: preparar la muestra de tu proyecto.

STOP: ¿Cerramos el taller a lo grande? /clase-4-3

USER: Sí / /clase-4-3

---

## Notas para Claude

- Las dos skills quedan creadas DE VERDAD, con frontmatter y descripción bien escrita
- El momento de la invocación automática (pedir la tarea con palabras normales y que la skill se dispare sola) es el corazón de la lección: no lo saltees ni lo cuentes, hacelo pasar
- Si después de reiniciar la skill no se dispara sola, casi siempre es la `description`: mejorala con las palabras que usa la persona y volvé a probar. Si igual no sale, invocala con /nombre y seguí sin dramatizar
- La tarea personal es lo que se lleva puesto: dedicale el tiempo que haga falta
- Sé honesto con los límites: las skills no se ejecutan solas de madrugada; MCP y programación de tareas son escalones siguientes

## Criterios de éxito

- [ ] Existe .claude/skills/prensa/SKILL.md y funciona
- [ ] Vio la skill dispararse SOLA, sin nombrar ningún comando
- [ ] Hizo su tarea real a mano una vez conmigo
- [ ] Existe la skill de SU tarea, y una copia en su carpeta personal (~/.claude/skills/)
- [ ] Se lleva la receta de 4 pasos y la regla ("no automatizar lo que no entendés")
