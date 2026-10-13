# prediccion_precios_viviendas_boston

Este proyecto implementa un flujo completo de aprendizaje automático para analizar y predecir los precios de las viviendas en Boston basándose en múltiples características socioeconómicas y geográficas del conjunto de datos clásico de la Universidad Carnegie Mellon (CMU).

## Contenido del Proyecto
- **Carga y preprocesamiento de datos:** Extracción y análisis exploratorio del conjunto de datos original (`Boston Housing`), comprobación de valores nulos y estudio de correlaciones.
- **Visualización:** Generación de gráficos de dispersión para identificar la relación crítica de variables clave como el número de habitaciones (`RM`) y el estatus socioeconómico (`LSTAT`) frente al precio (`MEDV`).
- **Modelado predictivo:**
  - **Regresión Lineal Simple:** Utilizando una única variable (`RM`).
  - **Regresión Lineal Múltiple:** Utilizando todas las características disponibles.
  - **Árboles de Regresión:** Experimentación con diferentes profundidades (`max_depth=2` y `max_depth=5`) para evaluar la mejora en el rendimiento.
  - **Predicción Multi-salida:** Aplicación de árboles de decisión para predecir simultáneamente el precio de la vivienda (`MEDV`) y el índice de criminalidad (`CRIM`).

*Nota:* Para una explicación analítica y detallada de los resultados, consulte la memoria en formato PDF incluida en este repositorio.