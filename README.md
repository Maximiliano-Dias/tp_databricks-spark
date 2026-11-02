# TP: Introducción a Databricks y procesamiento de datos con Apache Spark

Trabajo práctico de la materia **Análisis de datos en la nube**.

**Alumno:** Nombre Apellido

## Descripción
Se realizó un proceso ETL completo en Databricks Free Edition, usando Python, Spark SQL y Delta Lake, sobre un dataset de clubes del fútbol argentino.

## Dataset
- `equipos_futbol_argentino.csv`: 30 clubes con equipo, ciudad, provincia, año de fundación y estadio. Se incluyeron duplicados y valores nulos a propósito para practicar la limpieza.
- `provincias_regiones.csv`: tabla auxiliar que relaciona cada provincia con su región, usada para el join.

## Etapas realizadas
1. **Configuración del entorno:** notebook en Databricks con cómputo serverless.
2. **Carga y exploración:** lectura del CSV con Spark y consultas con Spark SQL.
3. **Transformaciones:** eliminación de duplicados, tratamiento de nulos, columnas calculadas (`antiguedad`, `epoca`), filtros, agregaciones y join con la tabla de regiones.
4. **Delta Lake:** almacenamiento de los datos transformados y validación de integridad.
5. **Visualización y análisis:** gráficos de clubes por provincia, por década de fundación y antigüedad promedio por región.

## Resultados principales
- Buenos Aires, CABA y Santa Fe concentran 21 de los 29 clubes analizados.
- La década de 1900 es la que más clubes fundó (16 de 29).
- La región Centro tiene la mayor antigüedad promedio (119,4 años).

## Archivos
- `TP_Databricks_Spark_Godoy_Dias.ipynb`: notebook con el código comentado y los resultados.
- `TP_Databricks_Spark_Godoy_Dias.html`: versión exportada para ver en el navegador.
- Archivos CSV con los datos de entrada.

## Aclaración
El dataset es una muestra armada para el trabajo práctico, no un listado oficial. Los años de fundación deberían verificarse con fuentes oficiales si se usan fuera de este contexto.
