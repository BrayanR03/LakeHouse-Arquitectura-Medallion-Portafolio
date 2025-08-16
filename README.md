# 🪙 Medallion Architecture en Databricks Free Edition 2025

Este proyecto implementa la arquitectura **Medallion** en **Databricks Free Edition 2025**, 
aplicando buenas prácticas de gobierno de datos, limpieza, transformación y generación de métricas de negocio.  

La arquitectura Medallion se basa en **tres capas principales**:
- **Bronze**: Ingesta cruda.
- **Silver**: Limpieza y estandarización.
- **Gold**: Métricas y análisis de valor.

---

## 🏗️ Arquitectura Implementada

### 1️⃣ Bronze Layer
- Ingesta de datasets sin modificar.
- Validación rápida de la estructura.
- Identificación de valores nulos y tipos de datos.
- Almacenamiento en **Delta Tables** bajo Unity Catalog.

### 2️⃣ Silver Layer
- Limpieza de datos:
  - Eliminación de nulos.
  - Estandarización de campos de texto (ejemplo: quitar guiones, aplicar Capitalize).
- Organización de los datos en **Schemas**.
- Generación de datasets listos para consumo analítico.

### 3️⃣ Gold Layer
- Creación de métricas y reportes de negocio:
  - **Resumen por categorías** de ventas.
  - **Top 5 productos** con mayor monto de ventas.
  - **Ranking de productos** según volumen de ventas.
- Preparación para consumo en dashboards o analítica avanzada.

---

## 🔗 Trazabilidad entre capas

Gracias a **Unity Catalog** y el uso de **Delta Tables**, se garantiza:
- Auditoría y versionado de datos entre capas.
- Lineage claro: cada transformación tiene su origen trazable.
- Escalabilidad para futuros pipelines y métricas.

---

## ⚙️ Tecnologías Usadas

- **Databricks Free Edition 2025**
- **PySpark / Spark SQL**
- **Delta Lake**
- **Unity Catalog & Schemas**
- **Dataframes API** (manipulación y consultas sin editor SQL)

---

## 📊 Resultados Destacados

Ejemplos de salidas en la capa **Gold**:
- 📌 Resumen de ventas por categoría.
- 📌 Identificación de los 5 productos más vendidos por monto.
- 📌 Ranking global de productos con mayor impacto.
- 📌 Métricas listas para visualización en dashboards.

---

## ✍️ Autor

👤 **Brayan Neciosup**  
📘 Bitácora de aprendizaje en ingeniería de datos – Publicaciones en LinkedIn  
🔗 [Mi portafolio](https://bryanneciosup626.wixsite.com/brayandataanalitics)  
🐙 [GitHub](https://github.com/BrayanR03)

