# 🌍 Global Socio-Economic Segmentation: Cluster Analysis

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Pandas](https://img.shields.io/badge/Library-Pandas-150458)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

## 📋 Descripción del Proyecto

Este proyecto aplica técnicas de **Aprendizaje No Supervisado (Unsupervised Learning)** para categorizar países basándose en indicadores socioeconómicos y de salud. 

Simulando un escenario de negocio para una entidad como el **Banco Mundial** u organizaciones no gubernamentales (ONGs), el objetivo es identificar grupos de países (clusters) con características similares para determinar la asignación estratégica de fondos y ayudas internacionales. A diferencia de los enfoques tradicionales, este modelo no utiliza etiquetas predefinidas, sino que descubre patrones latentes en los datos macroeconómicos.

## 🎯 Objetivo del Negocio

Identificar clusters de países (ej. "Necesitan Ayuda Urgente", "En Transición", "Economías Consolidadas") utilizando un enfoque puramente basado en datos (Data-Driven) para:
1.  Optimizar la asignación de recursos internacionales.
2.  Entender la correlación multidimensional entre variables de salud y economía.
3.  Proponer recomendaciones políticas diferenciadas por segmento.

## 📊 Sobre el Dataset

El conjunto de datos proviene de [Kaggle: Unsupervised Learning on Country Data](https://www.kaggle.com/datasets/rohan0301/unsupervised-learning-on-country-data) e incluye métricas clave para 167 países:

| Variable | Descripción |
| :--- | :--- |
| **child_mort** | Muerte de niños menores de 5 años por cada 1000 nacimientos. |
| **exports** | Exportaciones de bienes y servicios per cápita (% del PIB). |
| **health** | Gasto total en salud per cápita (% del PIB). |
| **imports** | Importaciones de bienes y servicios per cápita (% del PIB). |
| **income** | Ingreso neto per cápita. |
| **inflation** | Medida de la tasa de crecimiento anual del PIB total. |
| **life_expec** | Esperanza de vida al nacer (años). |
| **total_fer** | Tasa de fertilidad (número de hijos por mujer). |
| **gdpp** | PIB per cápita (Producto Interno Bruto). |

## ⚙️ Metodología (Pipeline)

El proyecto sigue un flujo de trabajo riguroso de Data Science:

1.  **Análisis Exploratorio de Datos (EDA):** Análisis univariado y bivariado, detección de outliers y mapas de calor de correlación.
2.  **Preprocesamiento:** Estandarización de datos utilizando `StandardScaler` para mitigar el sesgo de varianza entre variables (ej. Inflación vs PIB).
3.  **Reducción de Dimensionalidad (PCA):** Aplicación de Análisis de Componentes Principales para reducir el espacio dimensional y visualizar patrones en 2D/3D.
4.  **Modelado (Clustering):**
    * Determinación del número óptimo de clusters ($k$) mediante el **Método del Codo (Elbow Method)** y **Silhouette Score**.
    * Implementación del algoritmo **K-Means**.
5.  **Interpretación Económica:** Análisis de los perfiles resultantes (Profiling) para etiquetar los clusters según su realidad económica.

## 🛠 Herramientas Utilizadas

* **Lenguaje:** Python
* **Manipulación de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn (KMeans, PCA, StandardScaler)

---
*Autor: Luis Mauricio Aguirre Stornaiuolo*
*Estudiante de Economía | Universidad Nacional Mayor de San Marcos (UNMSM)*
