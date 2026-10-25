# Sistema de Monitoreo y Control Portuario (`port_log`)

**Sprint de Trabajo:** Sprint 3 (Integración de Datos y Modelado ORM)

---

## Introducción y Contexto

En el marco del desarrollo de la plataforma de gestión para la autoridad portuaria, el sistema `port_log` centraliza y procesa información operativamente crítica sobre el tráfico marítimo y los controles de velocidad en muelles. 

Durante los sprints previos se llevaron a cabo el procesamiento del registro de movimientos de buques (Sprint 1) y el análisis de calidad e identificación visual de patentes mediante procesamiento de imágenes (Sprint 2). En este **Sprint 3**, el enfoque se centra en la integración de ambas fuentes de datos mediante un modelo relacional persistido en base de datos con **SQLAlchemy**, gestionando el control de versiones del conjunto de datos con **DVC**.

---

## Objetivo

El objetivo principal de este sprint es consolidar el pipeline integrador de datos portuarios mediante:

1. **Persistencia con ORM:** Mapear e insertar las entidades `Buque`, `Radar`, `Movimiento` y `Evidencia` en la base de datos a partir de los datos procesados del puerto.
2. **Gestión de Radares Móviles:** Implementar consultas analíticas complejas que contabilicen los movimientos e infracciones registrados por radares móviles a lo largo de diferentes muelles.
3. **Control de Versionado de Datos:** Vincular el almacenamiento remoto (Supabase S3) con DVC para garantizar la trazabilidad de los artefactos y datasets del proyecto.
