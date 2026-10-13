# prediccion_precios_viviendas_boston

Este proyecto implementa un flujo completo de aprendizaje automático para analizar y predecir los precios de las viviendas en Boston basándose en múltiples características socioeconómicas y geográficas del conjunto de datos clásico de la Universidad Carnegie Mellon (CMU).


---

## Fases del Análisis

### 1. Carga y Preprocesamiento de Datos
Extracción y análisis exploratorio del conjunto de datos original (`Boston Housing`), comprobación de valores nulos y estudio de correlaciones de los atributos frente al precio (`MEDV`).

### 2. Visualización de Variables Críticas
Generación de gráficos de dispersión con líneas de tendencia para identificar la relación de variables clave como el número de habitaciones (`RM`) y el estatus socioeconómico (`LSTAT`) frente al precio.

### 3. Modelado Predictivo: Regresión Lineal Simple y Múltiple
- **Regresión Lineal Simple:** Utilizando únicamente la variable de habitaciones (`RM`).
- **Regresión Lineal Múltiple:** Utilizando todas las características disponibles del conjunto de datos.

### 4. Modelado Predictivo: Árboles de Regresión y Multi-salida
- **Árboles de Regresión:** Experimentación con diferentes profundidades (`max_depth=2` y `max_depth=5`) para evaluar la mejora en el rendimiento y métricas de error.
- **Predicción Multi-salida:** Aplicación de árboles de decisión para predecir simultáneamente múltiples variables objetivo (precio de la vivienda `MEDV` e índice de criminalidad `CRIM`).

*Nota:* Para una explicación analítica y detallada de los resultados, consulte la memoria en formato PDF incluida en este repositorio.

---

## Requisitos de Librerías
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`