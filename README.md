# 📊 Análisis Exploratorio & Correlacional — NovaRetail+

[![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://colab.research.google.com/drive/1P3fKOE2kA3Z7m-c_fwBwXZx4JoGvXWk5?usp=sharing)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)](https://scipy.org/)

## 🎯 Objetivo del Proyecto
Identificar los factores del comportamiento de los clientes más fuertemente asociados con el **ingreso anual generado** en **NovaRetail+**, analizando una base de **15,000 usuarios** y evaluando métricas clave como interacción en la plataforma, membresía Premium, satisfacción y tasa de abandono (*churn*).

---

## 🛠️ Tech Stack & Métodología
* **Data Prep & Cleaning:** Python (Pandas, NumPy) para auditoría de tipos de datos, limpieza y casting de variables.
* **Estadística & Correlaciones:** SciPy y Seaborn para la evaluación de relaciones lineales e inferenciales mediante:
  * **Pearson & Spearman:** Para variables numéricas (Compras vs. Ingreso anual, Publicidad vs. Visitas).
  * **Punto-Biserial & V de Cramér:** Para analizar asociación entre variables categóricas y continuas (Membresía, Abandono, Dispositivo y Región).

---

## 📊 Principales Hallazgos & Resultados

| Relación / Factor | Coeficiente | Hallazgo Clave |
| :--- | :---: | :--- |
| **Compras vs. Ingreso Anual** | **$r = 0.97$** | Correlación extremadamente alta. Requiere validación de arquitectura de datos para descartar multicolinealidad. |
| **Publicidad vs. Visitas Mensuales** | **$r = 0.58$** | Relación positiva moderada entre la inversión publicitaria y el tráfico generado. |
| **Satisfacción vs. Ingreso** | **$r \approx 0.00$** | Sin relación lineal directa; la calificación del cliente no determina su nivel de gasto. |
| **Membresía Premium vs. Abandono** | *Asociación débil* | Los usuarios Premium presentan menor tasa de abandono (*churn*) que los no afiliados. |

---

## 💡 Conclusiones del Negocio & Habilidades Demostradas

### 📌 Impacto de Negocio
* **Validación Crítica de Métricas:** Se identificó un posible sesgo metodológico en la variable `ingreso_anual` dada su altísima correlación ($r = 0.97$) con las compras mensuales, recomendando auditar la construcción del dataset antes de tomar decisiones de inversión.
* **Estrategia de Fidelización:** Aunque la retención es mayor en clientes Premium, la baja correlación entre la satisfacción reportada y el gasto demuestra la necesidad de replantear las encuestas de satisfacción (CSAT/NPS) hacia métricas accionables.

### 🧠 Capacidades Técnicas Demostradas
* **Rigor Estadístico Multivariado:** Selección y aplicación del coeficiente estadístico adecuado (Pearson, Spearman, Punto-biserial, V de Cramér) según la naturaleza de cada variable.
* **Análisis Exploratorio End-to-End:** Capacidad para estructurar un pipeline analítico claro desde la exploración sin nulos hasta la extracción de conclusiones orientadas a retención y crecimiento.

---

## 🔗 Enlaces del Proyecto

💻 **[Ejecutar Notebook en Google Colab](https://colab.research.google.com/drive/1P3fKOE2kA3Z7m-c_fwBwXZx4JoGvXWk5?usp=sharing)**

📁 **[Explorar Código y Archivos en el Repositorio](./)**

---
