# evaluacion_clasificacion_riesgo_industrial

Este repositorio contiene la resolución del examen práctico enfocado en técnicas de aprendizaje automático para la clasificación y evaluación de riesgos industriales.

---

## Contenido del Proyecto
- **Archivos de Datos:**
  - `manufacturing_risk_assessment.csv`: Dataset principal con variables de sensores y operación de motores para la evaluación del nivel de riesgo.
  - `predicciones_modelos_c.csv`: Archivo auxiliar con las predicciones generadas por diferentes modelos frente a la clase real.
- **Cuaderno Principal (`AAG_Examen.ipynb`):** Contiene el desarrollo analítico estructurado en fases para abordar tanto la exploración y preprocesamiento como la evaluación comparativa de modelos.

---

## Fases del Análisis

### 1. Carga de Datos y Análisis Exploratorio
Se cargan los datos de evaluación de riesgos y se realiza una inspección inicial mediante resúmenes estadísticos y verificación de valores nulos.

### 2. Detección y Análisis de Outliers (Valores Atípicos)
Se identifican y analizan los valores atípicos en las variables críticas (como la corriente del motor) utilizando metodologías basadas en diagramas de caja, el Rango Intercuartílico (IQR) y puntuaciones Z-Score.

### 3. Preparación y División del Conjunto de Datos
Se separan las variables predictoras de la variable objetivo (`risk_level`) y se realiza la división de los datos en conjuntos de entrenamiento y prueba.

### 4. Modelado Predictivo e Hiperparámetros
Se entrena un árbol de decisión inicial frente a un clasificador trivial (`DummyClassifier`) y se optimizan los hiperparámetros de profundidad máxima mediante validación cruzada y búsqueda en rejilla (`GridSearchCV`).

### 5. Evaluación Comparativa de Modelos
Se analizan múltiples modelos predictivos a través de matrices de confusión, informes de clasificación, tasas de error, métricas detalladas por clase (Precision, Recall y F1-score) y tasas de verdaderos y falsos positivos (TPR y FPR).

---

## Requisitos de Librerías
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `scipy`lisis y comparación de múltiples modelos predictivos a través de matrices de confusión, informes de clasificación, tasas de error, métricas detalladas por clase (Precision, Recall y F1-score) y cálculo de tasas de verdaderos y falsos positivos (TPR y FPR).