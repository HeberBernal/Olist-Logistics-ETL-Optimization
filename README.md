# Olist-Logistics-ETL-Optimization
"Pipeline de ETL y diagnóstico de integridad referencial para Olist. Análisis de eficiencia logística y rentabilidad mediante el cálculo de Densidad Económica por categoría."
# Olist Logistics: ETL & Optimization (Phase 1)

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data_Manipulation-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Business Intelligence](https://img.shields.io/badge/Business-Intelligence-FFD700?style=for-the-badge)

## 📋 Descripción del Proyecto
Este repositorio constituye la **Fase 1** de un análisis integral sobre el ecosistema de datos de Olist, el marketplace más grande de Brasil. El objetivo central es transformar un esquema relacional complejo en una **Fuente Única de Verdad (Single Source of Truth)** para diagnosticar la salud financiera y operativa de las transacciones.

A diferencia de un análisis convencional, este proyecto aplica rigor científico para identificar fugas de rentabilidad mediante el cruce de métricas logísticas y comerciales.

## 🚀 Hallazgos Estratégicos (Insights)
* **Densidad Económica:** Mediante el desarrollo del KPI de **Valor por Gramo ($/g)**, se identificó que categorías como *Watches Gifts* son hasta 12 veces más eficientes logísticamente que *Housewares*.
* **Anomalías de Costo:** Detección de "Zonas de Pérdida" donde el valor del flete supera el precio del producto, comprometiendo el margen neto.
* **Sesgo de Servicio:** Identificación de fallos críticos en la cadena de suministro con retrasos superiores a los 180 días, analizados mediante el Coeficiente de Variación (CV).

## 🛠️ Metodología Técnica

### 1. Ingeniería de Datos (ETL)
* **Unión Relacional:** Integración de múltiples datasets (`orders`, `products`, `order_items`, `translations`) asegurando la integridad referencial.
* **Auditoría de Calidad:** Implementación de funciones automatizadas para el escaneo de nulos y validación de tipos de datos en la fuente.

### 2. Diagnóstico de Ruido y Estandarización
* **Limpieza Semántica:** Estandarización de categorías y tratamiento de nulos mediante imputación por mediana.
* **Validación Temporal:** Detección y filtrado de inconsistencias en el sistema (fechas de entrega previas a la compra).

### 3. Análisis Estadístico Avanzado
* **Gestión de Outliers:** Uso de metodología robusta (**IQR**) para segmentar el comportamiento de precios y pesos.
* **KPIs de Rendimiento:** Desarrollo de métricas personalizadas como `delivery_time` (eficiencia real) y `delta_vs_estimated` (cumplimiento de promesa).

## 📂 Estructura del Repositorio
* `Análisis_EDA_... .ipynb`: Notebook principal con el flujo completo de ETL y visualizaciones estratégicas.
* `README.md`: Documentación del proyecto y hallazgos.

---
**Siguiente Paso:** [Fase 2 - Modelo Predictivo de Machine Learning]

**Desarrollado por:** Heber Job Bernal Monarrez  
*Especialista en Análisis de Datos y Ciencias Biomédicas*
