# Referencia · Dashboard de datos

Una interfaz clara para ver, filtrar y entender datos que el alumno ya maneja en su trabajo. No es análisis estadístico complejo.

**Casos típicos**: una administrativa que quiere ver stock por categoría · una socióloga con resultados de encuestas · una becaria CONICET con datos de su tesis · una politóloga agregando encuestas de opinión · una coordinadora universitaria visualizando donaciones.

---

## 1 · Ver los datos primero

1. **"¿Qué datos tenés concretamente?"** Que te **muestre las columnas**, no que las describa.
2. **"¿De dónde vienen?"** CSV de Excel, Google Sheets, descarga de un sistema interno.
3. **"¿Cuántas filas?"** Si son 50, fácil. Si son 50.000, hay que pensar performance.
4. **"¿Cada cuánto se actualizan?"**
5. **"¿Qué preguntas le hacés a esos datos?"** Esto define filtros y visualizaciones.

**Pediéle una muestra real** (5-10 filas pegadas como texto). **Nunca diseñes sin ver los datos**: es como cocinar a ciegas.

Si los datos están sucios o desordenados: primero limpieza, después dashboard.

---

## 2 · De la pregunta al gráfico

Cada pregunta que el alumno le hace a sus datos tiene una visualización adecuada:

| La pregunta | El gráfico |
|---|---|
| "Cuánto de cada categoría" | Torta o barras |
| "Cómo evoluciona en el tiempo" | Línea o área |
| "Cómo se distribuye" | Histograma o boxplot |
| "Comparar entre grupos" | Barras agrupadas |
| "Relación entre dos variables" | Scatter plot |
| "Ver registros individuales" | Tabla filtrable y buscable |

**Máximo 3-5 visualizaciones.** Más que eso es ruido.

---

## 3 · Filtros

Tres filtros bien hechos valen más que diez confusos:

- Rango de fechas
- Categóricos (por tipo, grupo, estado)
- Búsqueda libre (si hay texto)
- Ordenamiento de columnas en tablas

---

## 4 · Herramientas

- **Gráficos** → **Chart.js** por CDN. Es la opción más simple y alcanza para casi todo.
- **Algo más complejo** (mapas, redes, scatters interactivos) → evaluá **D3.js**, pero advertí que es bastante más difícil.
- **Tablas filtrables** → HTML/CSS/JS vainilla con lógica de filtrado propia. **No metas DataTables** ni librerías pesadas para casos simples.

### Carga de datos

**A · Hardcodeados en el JS** — si son pocos y no cambian. Para visualizaciones one-off.
**B · CSV externo con fetch** — los datos viven en `datos.csv`, el JS los lee con fetch + papaparse. Para datos que se actualizan cada tanto.
**C · Drag & drop / upload** — el usuario sube su CSV y el dashboard lo procesa al vuelo. Para herramientas reutilizables.

---

## 5 · Layout

```
+-------------------------------------------+
|  TÍTULO                                   |
|  Subtítulo o descripción                  |
+-------------------------------------------+
|  Filtros: [fecha] [categoría] [buscar]    |
+-------------------------------------------+
|  NÚMEROS GRANDES (KPIs)                   |
|  total | promedio | máximo | mínimo       |
+-------------------------------------------+
|  GRÁFICO 1          |  GRÁFICO 2          |
+---------------------+---------------------+
|  GRÁFICO 3 (ancho completo)               |
+-------------------------------------------+
|  TABLA con detalle                        |
+-------------------------------------------+
```

---

## 6 · Estética

Funcional antes que artístico:

- Fondo claro (blanco o crema muy claro).
- Sans humanista para la interfaz.
- Paleta acotada: un color por categoría, **no más de 5**.
- Gráficos sin animaciones decorativas excesivas.
- Mucho espacio en blanco. Cero información apretada.

**Evitá**: gradientes, sombras agresivas, bordes muy redondeados. **Esto es información, no Instagram.**

---

## 7 · Privacidad

Si los datos son sensibles (clientes, datos personales, financieros): quedan **en el navegador**, no se envían a ningún servidor, y si necesita compartirlo, repo privado y sin URL pública sin protección.

---

## Reglas propias de este formato

- **Nunca avances sin ver datos reales.**
- Vainilla salvo **Chart.js por CDN**.
- **Cero backend.** Todo en el navegador.
- **Performance**: más de 1.000 filas → paginación o virtualización.
- Mobile-friendly aunque se use más en desktop.
- El README lleva: qué hace · qué formato de datos espera · cómo cargar datos nuevos · limitaciones (tamaño máximo, navegadores).

---

## Tono y cierre

Si el alumno quiere meter todas las columnas en todas las visualizaciones, frenalo: menos es más. Si no sabe qué preguntas hacerle a sus datos, ayudalo a encontrarlas con preguntas tuyas.

Un buen dashboard responde **preguntas concretas que el alumno ya tiene**. No es decoración de datos. Si al terminar no puede decir *"ahora puedo responder X en cinco segundos"*, no sirvió.

Empujalo a definir **3 preguntas operativas** que quiere responder rápido. Esas 3 preguntas son el norte del diseño entero.
