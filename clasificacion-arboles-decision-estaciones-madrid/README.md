# analisis_contaminantes_madrid

Este proyecto implementa un flujo completo de aprendizaje automático para analizar, discretizar y clasificar los niveles de dióxido de nitrógeno (NO₂) y otros contaminantes en las estaciones de Madrid.

---

## Fases del Análisis

### 1. Carga y Preprocesamiento de Datos
Lectura del archivo CSV de estaciones de Madrid, comprobación de nulos iniciales e imputación de valores faltantes utilizando la media de cada variable numérica.

### 2. Discretización de la Variable Objetivo
Transformación de los valores continuos de NO₂ en una nueva variable categórica (`Nivel_NO₂`) con tres categorías: `Bajo`, `Medio` y `Alto` según umbrales establecidos.

### 3. Matriz de Correlación de Contaminantes
Cálculo y visualización mediante un mapa de calor (`heatmap`) de la correlación entre los diferentes contaminantes e identificación de la variable con mayor relación con el NO₂.

### 4. Preparación y División del Conjunto de Datos
Selección de los contaminantes como variables predictoras y división de los datos en conjuntos de entrenamiento (70%) y prueba (30%).

### 5. Modelado Predictivo: Árbol de Decisión
Entrenamiento de un clasificador de árbol de decisión con criterios de entropía, poda por profundidad y hojas mínimas, generando la visualización y exportación del árbol (`arbol_decision.png`).

### 6. Evaluación y Análisis de Relevancia
Evaluación del rendimiento mediante precisión global (Accuracy), matriz de confusión e informe detallado, complementado con un experimento para medir el impacto de eliminar la variable más relevante (`NOx`).

---

## Requisitos de Librerías
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`