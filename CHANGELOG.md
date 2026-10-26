[Ejercicio 09]
- Se redacta la conclusión integradora de los 3 sprints.

[Ejercicio 08]
- Se implementa buscar_buque_por_imagen con OpenCLIP y ChromaDB.
- Se recuperan buque, movimientos y evidencias desde la base relacional.
- Se advierte cuando la imagen es un plate o la similitud es baja.

[Ejercicio 07]
- Se crea la base vectorial buque_vectorial con ChromaDB y OpenCLIP.
- Un embedding por buque, desde su imagen complete de mayor ratio.

[Ejercicio 06]
- Se implementan 6 consultas SQLAlchemy sobre transito_portuario.
- Top buques, movimientos sin evidencia, radares, reincidentes, exceso por muelle y cobertura de evidencia.

[Ejercicio 05]
- Se crea la base transito_portuario con SQLAlchemy (SQLite).
- Se migra port_movements_image.csv usando procesar_fila_csv.

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

[Ejercicio 01]
- Se crea la rama Sprint_3 a partir de Sprint_2.
- Se verifica el acceso a los datasets de los sprints anteriores.
- Se actualiza README.md con el sprint actual, objetivo y contexto.

