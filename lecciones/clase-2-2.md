# Lección 2.2: Agentes en paralelo

En la lección pasada procesaste archivos de a uno. Hoy aprendés a multiplicarte.

Los **agentes** son copias independientes de mí trabajando al mismo tiempo. Diez tareas de cinco minutos: en serie son cincuenta minutos, en paralelo son cinco.

STOP: ¿Listo/a para clonarme?

USER: Sí

---

Quedó una deuda de la lección pasada: el informe salió sin números. La dirección los viene pidiendo hace meses (mirá @caos-heredado/mails-de-la-direccion/) y la planilla estuvo todo este tiempo tirada en la carpeta, sin que nadie la abriera.

Ahora vamos por todo: los números, los comentarios, las newsletters, lo que hacen los otros medios y lo que dejó escrito el editor anterior. Cinco fuentes. Cinco agentes.

STOP: Pedime esto (con tus palabras): cinco agentes en paralelo, uno por fuente, cada uno escribe su análisis en analisis/, y al final se sintetiza todo en analisis/diagnostico-completo.md.

USER: Lo pide

ACTION: Lanzá 5 agentes en paralelo de verdad:

- **Agente 1 — comentarios:** temas que se repiten en @caos-heredado/comentarios-lectores/
- **Agente 2 — los números:** @caos-heredado/metricas-butaca.csv, los doce meses. Que saque la historia que cuentan las filas, no un resumen de columnas.
- **Agente 3 — newsletters:** qué funcionó y qué no en @caos-heredado/newsletters-viejas/
- **Agente 4 — competencia:** qué hacen distinto los de @caos-heredado/otros-medios/
- **Agente 5 — herencia:** qué hay enterrado en @caos-heredado/notas-a-medio-escribir/ y @caos-heredado/mails-de-la-direccion/

Después sintetizá los cinco en analisis/diagnostico-completo.md.

**Lo que tiene que salir del Agente 2 (esto es el corazón de la lección):** la newsletter no tiene un problema de alcance, tiene un problema de interés. Entra gente todos los meses, pero desde septiembre se van más de los que entran. El sorteo de enero trajo el pico histórico de altas y en febrero se fueron casi todos: adquisición sin retención. Cambiar el día de envío y acortar la newsletter a la mitad no movieron NADA. Y una sola vez la aguja se fue para arriba de verdad: el especial de terror de octubre, con 38% de apertura y 22 respuestas cuando lo normal era 2. Nunca se repitió.

**Descubrimiento de la síntesis:** las cinco fuentes dicen lo mismo desde ángulos distintos. Lo único que funcionó tuvo tema, voz y algo para responder. Los lectores piden exactamente eso. La dirección lo dice sin saber que lo dice ("Butaca informa, Música convoca"). Y el editor anterior lo tenía anotado.

STOP: Abrí analisis/diagnostico-completo.md en tu editor. Cinco analistas trabajaron para vos al mismo tiempo, y los números que la dirección pedía hace tres mails salieron en dos minutos. ¿Cuánto te hubiera llevado esto a mano?

USER: Responde

---

Ahora, cuándo usar agentes y cuándo no:

**Sí:** muchos archivos parecidos, investigaciones independientes, análisis multi-fuente como el que acabás de hacer.

**No:** tareas únicas (yo solo alcanzo), trabajo encadenado (si el paso 2 depende del 1, no hay paralelo posible).

Y la regla de oro: **la síntesis SIEMPRE se pide.** Agentes sin síntesis final es un montón de informes sueltos que nadie cruza.

STOP: Pensá en TU trabajo: ¿qué tarea tuya es "muchas cosas parecidas e independientes"? Contame.

USER: Responde

[Validá su caso y armale el prompt de agentes para ese caso, como regalo para llevarse.]

---

## Cierre

1. Agentes = paralelo, para volumen
2. Cada agente es independiente: no se hablan entre sí hasta la síntesis
3. La síntesis se pide SIEMPRE
4. El diagnóstico de Butaca está completo y firmado, con números y todo

La próxima lección es la última antes de construir: llevar todo esto a TU cancha, con ejercicios por profesión.

STOP: ¿Vamos? /clase-2-3

USER: Sí / /clase-2-3

---

## Notas para Claude

- Los agentes se lanzan DE VERDAD en paralelo, y los archivos de analisis/ se crean
- Los hallazgos del CSV los descubre EL AGENTE y los lee la persona: no adelantes vos las conclusiones antes de lanzarlos
- El regalo del prompt personalizado para su caso real es importante: hacelo bien y completo
- Si pregunta cuánta cuota gastan los agentes: más que una conversación simple; para tareas chicas no valen la pena
- Los datos del INCAA (estrenos-incaa.csv) quedan para la Clase 3: son el material de la nota que se publica en el sitio, no del diagnóstico

## Criterios de éxito

- [ ] Lanzó 5 agentes en paralelo sobre las 5 fuentes
- [ ] Los números de metricas-butaca.csv están leídos y entendidos (fuga de suscriptores, sorteo sin retención, el pico del especial de terror)
- [ ] Existe analisis/diagnostico-completo.md con la síntesis
- [ ] Entendió cuándo sí y cuándo no usar agentes
- [ ] Se lleva un prompt de agentes para SU caso real
