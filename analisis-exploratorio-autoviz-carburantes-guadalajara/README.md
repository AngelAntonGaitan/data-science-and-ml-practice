# Análisis Exploratorio de Precios de Carburantes en Guadalajara

Este proyecto realiza un análisis exploratorio de datos (EDA) y preprocesamiento de precios de carburantes en la provincia de Guadalajara a partir de un conjunto de datos en formato CSV, empleando la librería `AutoViz` para la generación automática de visualizaciones.

---

## Contenido del Repositorio
- **Conjunto de datos original**: Archivo CSV con los registros de precios de carburantes.
- **Cuaderno de Jupyter**: Contiene el flujo completo de preprocesamiento, limpieza y análisis.
- **Documento PDF**: Memoria de entrega final de la actividad.

---

## Configuración del Entorno
El proyecto requiere la instalación y fijación de versiones específicas de librerías para asegurar la compatibilidad y evitar conflictos de dependencias en el entorno virtual de Python.

---

## Fases del Análisis

### 1. Carga y Filtrado Geográfico
Se realiza la lectura del archivo CSV asegurando la codificación adecuada, la limpieza de los nombres de columnas y el filtrado exclusivo de los registros correspondientes a la provincia de Guadalajara.

### 2. Detección y Tratamiento de Valores Nulos
Se identifican las columnas con datos faltantes, se convierten los precios a formato numérico (reemplazando comas por puntos decimales) y se imputan los valores nulos utilizando la media de cada variable.

### 3. Análisis de Outliers (Valores Atípicos)
Se aplica una metodología basada en el Rango Interquartílico (IQR) para detectar, analizar y filtrar los valores atípicos en los precios de los carburantes.

### 4. Normalización de Variables
Se escalan las variables numéricas principales utilizando técnicas de normalización para unificar sus rangos de valores.

### 5. Limpieza de Tipos de Datos Categóricos
Se corrigen y homogeneizan los tipos de datos en columnas de texto, como el tipo de servicio ofrecido por las estaciones.

### 6. Visualización y Ejecución de AutoViz
Se generan gráficos de dispersión y tendencias para estudiar la correlación entre los diferentes carburantes, complementado con la ejecución del reporte automatizado mediante `AutoViz`.

---

## Requisitos de Librerías
- `pandas`
- `matplotlib`
- `seaborn`
- `autoviz`
- `xgboost`
- `scikit-learn`