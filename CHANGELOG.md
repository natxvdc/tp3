[Ejercicio 04]
- Se implementan los modelos Buque, Radar, Movimiento y Evidencia.
- Se completa procesar_fila_csv con reutilización de Buque y Radar.

[Ejercicio 03]
- Se diseña el modelo lógico: Buque, Radar, Movimiento y Evidencia.
- Se documentan atributos, claves y cardinalidades en reports.

[Ejercicio 02 - dataset procesado]
- Se versiona con DVC port_log/data/processed/port_movements_image.csv.

[Ejercicio 02 - gráficos]
- Se migran a DVC los gráficos de port_log/data/interim/plots.

[Ejercicio 02 - imágenes]
- Se configura DVC con Supabase como remoto S3.
- Se migran a DVC las imágenes de port_log/data/raw/imgs.

[Ejercicio 02 - gráficos]
- Se migran a DVC los gráficos de port_log/data/interim/plots.

# Registro de Cambios (Changelog)

## [Sprint 3] - 2026-10-25

[Ejercicio 06]
- Se modificó la consulta en SQLAlchemy para el reporte de radares más activos contabilizando la cantidad de muelles distintos (`func.count(func.distinct(Movimiento.muelle))`) en los que registró actividad cada dispositivo.

[Ejercicio 05]
- Se adaptó el análisis de imágenes sin match leyendo directamente desde el archivo CSV de resultados persistido en disco.

[Ejercicio 04]
- Se ajustó el print de validación de carga del CSV reemplazando `mov.radar.muelle` por la propiedad directa `mov.muelle`.

[Ejercicio 03]
- Se actualizó el modelo de dominio SQLAlchemy indicando que un radar es un dispositivo móvil que opera en distintos muelles ("Un movimiento ocurre en un único muelle").

[Ejercicio 02]
- Se reestructuró la validación y cálculo de dimensiones de imagen (ancho x alto) eliminando código duplicado de verificaciones.

[Ejercicio 01]
- Se integró el dataset filtrado del TP1 (`port_movements.csv`) con las métricas de detección de imágenes del TP2.
