# Sobre los datos de esta carpeta

**Todos son datos de práctica para el taller.** Verosímiles, pero inventados.

## metricas-butaca.csv

Los números propios de Butaca Semanal: doce meses de suscriptores, altas, bajas, aperturas, clics y respuestas, mes por mes.

Es la planilla que la dirección pidió tres veces y nadie mandó. La historia de por qué la newsletter se está muriendo se lee entera en estas doce filas, si alguien se sienta a mirarlas.

Columnas:
- `suscriptores`: total a fin de mes
- `altas` / `bajas`: entradas y salidas de ese mes
- `tasa_apertura_pct`: porcentaje de suscriptores que abrió (promedio del mes)
- `tasa_clic_pct`: porcentaje que clickeó algún link
- `respuestas`: cuántos lectores contestaron el mail
- `nota`: qué se probó ese mes

## estrenos-incaa.csv

Datos de la industria del cine argentino: estrenos, espectadores y cuota de pantalla nacional, de 2015 a 2025.

Las cifras siguen las tendencias reales (caída de espectadores, derrumbe 2020, recuperación parcial, cuota nacional en baja), pero están redondeadas e inventadas para el ejercicio.

**NO citar estas cifras en trabajos reales.** Los datos reales del INCAA están publicados en sus informes de gestión y en datos.gob.ar.

Columnas:
- `estrenos_totales`: películas estrenadas comercialmente en el año
- `estrenos_argentinos`: cuántas de esas son producciones nacionales
- `espectadores_totales`: entradas vendidas en el año (todas las películas)
- `espectadores_cine_argentino`: entradas vendidas para películas argentinas
- `cuota_pantalla_nacional_pct`: porcentaje de espectadores que eligió cine argentino
