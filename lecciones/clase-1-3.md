# Lección 1.3: Comandos y atajos

Esta lección es corta y práctica: los comandos que vas a usar todos los días y los atajos que te devuelven el control cuando algo se va de tema.

Los comandos que empiezan con `/` son órdenes directas para Claude Code (el programa), no para la conversación.

STOP: Escribí `/` (solo la barra) y mirá el menú que aparece. No elijas nada, solo espiá y contame qué ves.

USER: Describe el menú

Ese menú es todo lo que sé hacer. La buena noticia: necesitás siete u ocho de esos, no todos.

---

Los esenciales, en orden de importancia:

- `/clear`: conversación nueva de cero. Los archivos quedan, el chat se borra. Usalo cada vez que cambiás de tema: me mantiene enfocado y te ahorra cuota.
- `/compact`: cuando la conversación se hizo larga, resumo todo lo hablado y sigo con el resumen. La diferencia con `/clear`: `/clear` me borra la memoria de la charla, `/compact` la comprime y me la deja. Cuando te avise que me estoy quedando sin contexto, esta es la salida.
- `/rewind`: el botón de deshacer. Ya lo vemos en detalle en un minuto.
- `/resume`: retomar una conversación anterior después de cerrar.
- `/usage`: cuánta cuota llevás usada.
- `/doctor`: chequeo de salud si algo anda raro.
- `/help`: la lista completa.

STOP: Probá `/usage` ahora y contame qué ves.

USER: Lo prueba

---

Ahora los atajos de control. Estos son los que te hacen sentir al volante:

**La tecla ESC**: me frena en seco, en medio de lo que esté haciendo. Si ves que agarré para cualquier lado, frename sin culpa. No me ofendo.

**Rebobinar**: el viaje en el tiempo. Guardo una foto de tus archivos antes de cada edición, y una más con cada mensaje que me mandás. Al rebobinar elegís un momento del pasado y volvés.

Y volvés **qué**, exactamente: acá hay dos líneas de tiempo que corren en paralelo, la **conversación** (lo que hablamos) y los **archivos** (lo que quedó escrito). Rebobinar es elegir cuál de las dos volvés para atrás: las dos juntas (lo más común, como si nada hubiera pasado), solo los archivos (deshacés lo escrito pero me sigo acordando de todo), o solo la conversación (me olvido de la charla y los archivos quedan como están).

[Dale el gesto de SU superficie, según la tabla de superficies:
- Terminal: `/rewind`, o la tecla ESC dos veces con el campo de texto vacío (si hay texto escrito, el doble ESC borra ESO en vez de abrir el menú).
- Panel de VS Code: pasar el mouse por encima de un mensaje anterior y clickear el botón de rewind que aparece.
- Desktop: probar `/rewind` en la lista de comandos; si no aparece, ser honesto y decir que en Desktop la red de seguridad es Git (Clase 3).]

Y el límite, que es importante: rebobinar **no deshace todo**. No revierte lo que se hizo por comandos de terminal, ni los cambios que hiciste vos a mano por fuera. Es un "deshacer" de sesión, no un respaldo. El respaldo de verdad es Git, y lo vemos en la Clase 3.

STOP: Esto es lo que te deja experimentar sin miedo: si algo sale mal, rebobinás. Abrí el menú de rebobinado ahora, mirá las opciones y salí sin tocar nada. ¿Lo viste?

USER: Confirma

**Los modos de trabajo**: son tres, y definen cuánto permiso me das.
- **Normal**: te pido permiso antes de cada cambio (el default, ideal mientras aprendés)
- **Auto-accept**: hago todo sin preguntar (para cuando ya confiás)
- **Plan**: primero armo un plan, vos lo aprobás, después ejecuto (para tareas grandes)

[Gesto según superficie: en la terminal, Shift+Tab rota entre los tres. En el panel de VS Code, se clickea el indicador de modo abajo del campo de texto. En Desktop, el selector al lado del botón de enviar (Ctrl/Cmd+Shift+M).]

STOP: Cambiá de modo un par de veces y mirá cómo cambia el indicador. Dejalo en Normal cuando termines. ¿Lo ves?

USER: Confirma

---

Dos yapas de poder:

**Palabras de pensamiento:** si me escribís `think`, `think harder` o `ultrathink` en un pedido, pienso más profundo. Sirve para decisiones complejas. Ojo: gasta más cuota, no lo uses para pavadas.

**Los comandos son archivos:** /clase-1-1 y compañía no vienen de fábrica: son archivitos de texto en `.claude/commands/`. En la Clase 4 vas a crear los tuyos: /informe, /prensa, lo que tu rutina necesite.

STOP: Pregunta de comprensión, sin trampa: ¿cuándo usarías el modo Plan en tu trabajo real?

USER: Responde con algún caso

[Validá su ejemplo o afiná: modo Plan = tareas grandes, con muchos pasos, donde querés revisar antes de que pase nada.]

---

## Cierre

Tu tablero de control:

| Qué | Terminal | Panel de VS Code | Desktop |
|-----|----------|------------------|---------|
| Frenar | ESC | ESC | ESC |
| Rebobinar | ESC ×2 o /rewind | Hover en el mensaje → botón | /rewind (si está); si no, Git |
| Cambiar modo | Shift+Tab | Clic en el indicador | Selector de modo |
| Conversación nueva | /clear | /clear | /clear |
| Comprimir contexto | /compact | /compact | /compact |
| Retomar | /resume | Historial de sesiones | Sidebar de sesiones |

[Mostrale la fila que le toca a ELLA/ÉL, no la tabla entera de memoria: la tabla completa está en el sitio del taller para el que quiera comparar.]

En la próxima lección le damos memoria a tu proyecto: el famoso CLAUDE.md.

STOP: ¿Vamos? /clase-1-4

USER: Sí / /clase-1-4

---

## Notas para Claude

- Los ejercicios de /usage, /rewind y Shift+Tab son de verdad: esperá a que los haga
- En el ejercicio de rewind, insistí en que salga con "Never mind": la idea es que vea el menú, no que rebobine la clase
- Si el doble ESC no le abre el menú, casi seguro tiene texto en el campo: que lo vacíe o que use /rewind
- Si pregunta por el "modo peligroso" (--dangerously-skip-permissions): existe, hace todo sin preguntar, y no es para la semana uno

## Criterios de éxito

- [ ] Vio el menú de /
- [ ] Probó /usage
- [ ] Abrió el menú de rewind y salió sin tocar nada
- [ ] Sabe que rewind no deshace lo que se hizo por terminal, y que Git es el respaldo real
- [ ] Sabe cuándo usar /clear y cuándo /compact
- [ ] Cicló los modos con Shift+Tab y volvió a Normal
- [ ] Puede decir cuándo usaría el modo Plan
