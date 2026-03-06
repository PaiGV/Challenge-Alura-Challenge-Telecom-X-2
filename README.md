## 📋 Descripción del Proyecto

Este proyecto utiliza técnicas de **Machine Learning** para identificar a los clientes con mayor probabilidad de cancelar sus servicios en la empresa de telecomunicaciones **Telecom X**. El objetivo es permitir que el equipo de marketing actúe proactivamente con campañas de retención.

## 🛠️ Tecnologías Utilizadas

* **Python** (Google Colab)
* **Pandas & NumPy**: Procesamiento y limpieza de datos.
* **Scikit-Learn**: Creación y evaluación de modelos de IA.
* **Seaborn & Matplotlib**: Visualización de datos y análisis exploratorio.

## 🚀 Pasos Realizados

### 1. Preparación y Limpieza

* Eliminación de variables irrelevantes 
* Tratamiento de valores nulos y conversión de tipos de datos.
* **Escalado de variables**: Se normalizaron para asegurar que los modelos basados en distancia no tuvieran sesgos.

### 2. Análisis Exploratorio (EDA)

* Se identificó que los clientes con **contratos mes a mes** y **altas cuotas mensuales** tienen una tasa de cancelación significativamente mayor.

### 3. Modelado

Se entrenaron y compararon dos modelos con una división de datos **80% entrenamiento / 20% prueba**:

1. **Regresión Logística**: Modelo sensible a la escala, optimizado con los datos normalizados.
2. **Random Forest**: Modelo basado en árboles, robusto frente a valores atípicos.

## 📈 Resultados

El modelo ganador fue la **Regresión Logística** con los siguientes resultados en el conjunto de prueba:

| Métrica | Valor |
| --- | --- |
| **Exactitud (Accuracy)** | **80%** |
| **Recall (Clase 1)** | **52%** |
| **F1-Score (Clase 1)** | **0.58** |

## 💡 Conclusiones y Estrategia

* **Hallazgo clave**: El tipo de contrato y el servicio de fibra óptica son los principales detonantes del abandono.
* **Recomendación**: Implementar alertas automáticas cuando un cliente con contrato mensual supere una cuota crítica, ofreciendo incentivos para migrar a contratos de largo plazo.


**¿Qué te parece?** Con este README tu proyecto de Alura pasará de "bueno" a "profesional". ¿Hay alguna otra sección que quieras añadir o ya estamos listos para el gran final?
