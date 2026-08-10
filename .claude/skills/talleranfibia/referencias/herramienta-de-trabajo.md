# Referencia · Herramienta de trabajo

Algo funcional que el alumno va a usar todos los días o todas las semanas para automatizar o facilitar una tarea concreta de su trabajo. No es un sitio ni una pieza autoral: es una herramienta.

**Casos típicos**: una docente que automatiza informes para alumnos · una administrativa con un panel de stock · una abogada con plantillas dinámicas de escritos · una periodista que gestiona entrevistas · una socióloga parlamentaria que redacta gacetillas · una marketinera que automatiza reportes para clientes.

---

## 1 · Entender la tarea

Las cinco preguntas, una por una:

1. **"¿Cuál es la tarea repetitiva que querés convertir en herramienta?"** Que la describa en detalle.
2. **"¿Cuánto tiempo te lleva hoy hacerla a mano?"** Para dimensionar el ahorro.
3. **"¿Qué inputs recibís?"** ¿Un Excel? ¿Un texto? ¿Datos de otra persona?
4. **"¿Qué output querés generar?"** ¿Un PDF? ¿Una página? ¿Un mensaje listo para enviar?
5. **"¿Hay datos sensibles?"** Clientes, alumnos, pacientes, casos legales.

**No avances sin las cinco respuestas claras.**

---

## 2 · Tipo de herramienta

**A · Formulario + generador de output**
El alumno completa campos, la herramienta genera un texto, PDF o mensaje listo. Para plantillas legales, informes docentes, gacetillas.

**B · Panel de control con datos**
Carga un CSV o ingresa datos, la herramienta muestra resúmenes y alertas. Para stock, ventas, seguimiento de proyectos. *(Si el foco es visualizar más que operar, mirá `dashboard-de-datos.md`.)*

**C · Asistente de texto**
Un input grande donde escribe contexto, la herramienta devuelve algo procesado. Para redacción asistida, análisis de textos, borradores.

**D · Plantilla con campos editables**
Campos completables que generan un documento final. Para contratos tipo, propuestas comerciales, presentaciones recurrentes.

Recomendá una, explicá por qué, confirmá.

---

## 3 · Estructura

**Todo en una sola página HTML autosuficiente** siempre que se pueda. La virtud de estas herramientas es que el alumno la abre en cualquier navegador sin instalar nada.

```
herramienta/
├── index.html      ← todo en un solo archivo
├── README.md       ← cómo se usa
└── ejemplos/       ← (opcional) archivos de ejemplo
```

Orden de construcción: HTML semántico → CSS sobrio → **JavaScript con la lógica** → validaciones → output limpio (descargable, copiable o exportable).

---

## 4 · Privacidad (crítico acá)

Si maneja datos sensibles, **decíselo explícitamente al alumno**, no lo asumas:

- Los datos **quedan en el navegador**, no se envían a ningún servidor.
- No se guardan en bases externas.
- Si necesita persistencia, `localStorage`.
- Si maneja datos confidenciales, **no la publiques en URL pública sin protección**.

Para herramientas con datos legales o de salud: repo privado en GitHub, o ejecutarla solo localmente.

---

## 5 · Estética

Funcionales, no artísticas. Clara, sobria, **no decorativa**.

**A · Administrativo limpio** — fondo blanco o gris muy claro, sans, paleta neutra con un acento. Tipo software interno bien hecho.

**B · Terminal moderno** — fondo oscuro, mono para inputs/outputs, colores funcionales (verde éxito, rojo error). Tipo herramienta de developer.

**C · Editorial funcional** — serif para títulos, sans para datos, mucho aire. Cercano a un editor de textos profesional.

---

## Reglas propias de este formato

- **Una sola página HTML** cuando sea posible.
- **`localStorage` para persistencia.** Cero backend.
- **Validaciones siempre.** Las herramientas profesionales no se rompen con inputs raros o vacíos.
- **Cero animaciones decorativas.** Esto es utilitario.
- **Mobile-first pero priorizando desktop** — estas herramientas se usan en computadora.
- El README lleva: qué hace · cómo se usa paso a paso con ejemplo · formato esperado de los inputs · limitaciones conocidas.

---

## Tono y cierre

Profesional pero accesible: suelen ser profesionales con poco tiempo. Concreto, sin vueltas — decí *"vamos a hacer"*, no *"podríamos considerar"*.

Si el alumno está perdido sobre qué automatizar, ofrecele ejemplos del tipo de herramienta que su perfil suele necesitar. Si quiere meter complejidad técnica innecesaria, frenalo: **las mejores herramientas son las más simples**.

Lo más importante no es que sea sofisticada, sino que **el alumno la use después del taller**. Una herramienta que se queda en una carpeta es un fracaso. Una herramienta fea que ahorra una hora por semana es un éxito.

Empujalo a diseñarla pensando en su Yo del próximo mes, no en mostrarla en un showcase. La métrica de éxito es una sola: **¿la abriste el lunes a la mañana?**
