# Análisis de datos

## ¿Qué hace un análista de datos?

Convierte preguntas de negocio en respuestas basadas en datos, y las comunica de forma que alguien pueda tomar una decisión.

- La gerente de marketing pregunta _"¿Por qué bajaron las ventas en la categoría moda del mes pasado?"_
- Se traduce la pregunta: ¿bajo el número de pedidos, el ticket promedio o ambos? ¿en todas las ciudades? ¿frente a que se compara?
- Se extraen los datos con SQL de la base de datos de la tienda
- Se limpian y exploran con Python/Pandas o Excel (nulos, duplicados, fechas mal escritas)
- Se encuentra que la caída se concentra en una ciudad y en clientes captados por publicidad pagada
- Se construyen 2-3 gráficos claros
- Se presenta: _qué paso, por qué creemos que pasó, qué recomendamos y qué no sabemos todavía_

## Ciclo de análisis: de la pregunta a la decisión

```
1. PREGUNTAR -> 2. OBTENER -> 3. LIMPIAR -> 4. EXPLORAR/ANALIZAR -> 5. COMUNICAR -> 6. ACTUAR Y MEDIR
```

| Paso | Que se hace | Ejemplo | Error típico |
|------|-------------|---------|--------------|
| 1. Preguntar | Se define una pregunta concreta medible y para quién es | ¿Que canal de adquisión trae clientes que más recompran | Empezar a graficar sin saber qué se quiere decidir |
| 2. Obtener | Conseguir los datos (SQL, archivos, API) | Exportar `clientes`, `pedidos`, `detalle_pedidos` | No verificar de dónde vienen ni que significan |
| 3. Limpiar | Corregir nulos, duplicados, formatos | Unificar "BOGOTÁ", "bogotá", "Bogotá" | Saltarse este paso (consume 50-80% del tiempo real) |
| 4. Explorar/Analizar | Resumenes, compras, buscar patrones y probar hipótesis | Recomprar por canal, ticket promedio por ciudad | Quedarse en el dato curioso sin conectarlo con la pregunta |
| 5. Comunicar | Contar la historia con gráficos y texto claro | Tablero de | página + 3 conclusiones | Mostrar todo lo que se hizo en vez de lo que importa |
| 6. Actuar y medir | Se toma una decisión y se mide su efecto | Reasignar presupuesto de publicidad y comparar 2 meses después | Entregar el reporte y desaparecer |