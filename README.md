# 📊 Predicción de Aprobación de Créditos mediante Machine Learning

## 📖 Descripción del Proyecto

Este proyecto fue desarrollado como parte de la asignatura **Ciencia de Datos con Python** de la Maestría. El objetivo es analizar un conjunto de datos de solicitudes de crédito mediante técnicas de análisis exploratorio de datos (EDA) y construir un modelo de **Machine Learning supervisado** que permita predecir la aprobación o rechazo de una solicitud de crédito.

El trabajo sigue un flujo completo de Ciencia de Datos, desde la carga y limpieza de los datos hasta la evaluación de un modelo predictivo utilizando Scikit-Learn.

---

## 🎯 Objetivo General

Desarrollar un modelo de Machine Learning supervisado que permita predecir la aprobación de créditos a partir de variables socioeconómicas y financieras de los solicitantes, apoyando la toma de decisiones basada en datos.

### Objetivos Específicos

- Realizar el análisis exploratorio del conjunto de datos para comprender su estructura y calidad.
- Preparar y transformar los datos mediante técnicas de limpieza y codificación de variables.
- Implementar y evaluar un modelo de clasificación utilizando Random Forest.

---

## 📂 Dataset

El proyecto utiliza el archivo:

```
creditos1.csv
```

El dataset contiene información de solicitudes de crédito, incluyendo variables como:

- Género
- Estado civil
- Dependientes
- Nivel educativo
- Trabajo independiente
- Ingresos del solicitante
- Ingresos del co-solicitante
- Monto solicitado
- Plazo del préstamo
- Historial crediticio
- Área de residencia
- Estado del crédito (variable objetivo)

---

## 🛠 Tecnologías Utilizadas

- Python 3
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-Learn

---

## 📚 Librerías Principales

```python
import pandas as pd
import numpy as np

import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px

from sklearn.model_selection import train_test_split
from sklearn.preprocessing import LabelEncoder

from sklearn.tree import DecisionTreeClassifier
from sklearn.ensemble import RandomForestClassifier

from sklearn.metrics import (
    accuracy_score,
    classification_report,
    confusion_matrix
)
```

---

## 🔄 Pipeline del Proyecto

```text
Carga del Dataset
        │
        ▼
Revisión Inicial
        │
        ▼
Limpieza de Datos
        │
        ▼
Transformación de Variables
        │
        ▼
Análisis Exploratorio (EDA)
        │
        ▼
Visualización de Datos
        │
        ▼
Entrenamiento del Modelo
        │
        ▼
Evaluación del Modelo
        │
        ▼
Conclusiones
```

---

## 📈 Análisis Exploratorio

Durante el EDA se realizaron las siguientes actividades:

- Revisión de estructura del dataset.
- Identificación de valores nulos.
- Eliminación de duplicados.
- Estadística descriptiva.
- Correlación entre variables.
- Análisis de variables categóricas.
- Creación de la variable **TotalIncome**.
- Visualizaciones estadísticas e interactivas.

---

## 🤖 Modelo de Machine Learning

### Tipo de problema

Clasificación Supervisada.

### Variable objetivo

```
Loan_Status
```

### Algoritmo utilizado

```
RandomForestClassifier
```

También se entrenó un Árbol de Decisión para comparar el desempeño de ambos modelos.

---

## 📊 Métricas Evaluadas

- Accuracy
- Precision
- Recall
- F1-Score
- Matriz de Confusión

---

## 📌 Principales Resultados

El modelo Random Forest obtuvo un desempeño superior al Árbol de Decisión, alcanzando una precisión aproximada del **76%**, lo que demuestra una adecuada capacidad para predecir la aprobación de créditos.

Las variables con mayor influencia fueron:

- Credit_History
- TotalIncome
- ApplicantIncome
- LoanAmount
- CoapplicantIncome

---

## 📁 Estructura del Proyecto

```
Proyecto_Creditos/

│
├── creditos1.csv
├── Notebook_Creditos.ipynb
├── Informe_Final.pdf
├── README.md
└── images/
      ├── pipeline.png
      ├── heatmap.png
      ├── histogram.png
      ├── boxplot.png
      └── importance.png
```

---

## 🚀 Cómo Ejecutar el Proyecto

1. Clonar el repositorio.

```bash
git clone https://github.com/usuario/proyecto-creditos.git
```

2. Instalar las dependencias.

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn
```

3. Abrir el notebook en Google Colab o Jupyter Notebook.

4. Ejecutar las celdas en orden.

---

## 📊 Resultados Esperados

El proyecto genera:

- Limpieza del dataset.
- Análisis exploratorio completo.
- Visualizaciones estadísticas.
- Modelo predictivo.
- Evaluación mediante métricas de clasificación.
- Importancia de variables.

---

## 📖 Conclusiones

El historial crediticio y los ingresos de los solicitantes fueron los factores más determinantes para la aprobación de créditos. El modelo Random Forest demostró ser una herramienta eficaz para apoyar la evaluación del riesgo crediticio y constituye una base sólida para futuras mejoras mediante técnicas más avanzadas de aprendizaje automático.

---

## 👨‍🎓 Autor

**Andrés Ñacato**

Proyecto desarrollado para la **Maestría** – Asignatura de Ciencia de Datos con Python.

---

## 📄 Licencia

Este proyecto tiene fines exclusivamente académicos.
