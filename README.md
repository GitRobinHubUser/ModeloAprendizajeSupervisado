# Actividad 3 - Métodos de Aprendizaje Supervisado
**Predicción del Tiempo de Viaje en TransMilenio usando Árboles de Decisión**

## Descripción del Proyecto
Este proyecto desarrolla un modelo de **aprendizaje supervisado** basado en un **Árbol de Decisión (DecisionTreeRegressor)** para predecir el tiempo de viaje entre estaciones del sistema TransMilenio de Bogotá.

El modelo se construye sobre el sistema de rutas con reglas lógicas y algoritmo A* desarrollado en la Actividad 2, logrando una excelente integración entre ambos enfoques.

**Referencia teórica principal:**  
Capítulo 17 – Aprendizaje de árboles y reglas de decisión  
Palma Méndez, J. T. (2008). *Inteligencia Artificial: Métodos, Técnicas y Aplicaciones*.

## Archivos del Repositorio
- `transmilenio_dataset.csv` → Dataset sintético con 1.500 registros
- `modelo_supervisado_transmilenio.ipynb` → Notebook Jupyter con el código completo
- `descripcion_datos.pdf` → Descripción detallada de los datos
- `pruebas_resultados.pdf` → Pruebas, métricas y análisis del modelo
- `arbol_decision_transmilenio.png` → Visualización del Árbol de Decisión
- `importancia_variables.png` → Gráfico de importancia de las variables

## Resultados del Modelo
- **Mean Absolute Error (MAE):** 2.57 minutos  
- **Root Mean Squared Error (RMSE):** 3.30 minutos  
- **R² Score:** 0.8575  

El modelo explica el **85.75%** de la variabilidad del tiempo de viaje.

**Variables más importantes:**
- `num_transbordos` (la más influyente)
- `tipo_hora_valle`
- `misma_troncal`

## Ejemplos de Predicción
- Héroes → Terminal (Autopista Norte): **67.5 minutos**
- Portal Suba → Portal Usme: **90.7 minutos**
- Portal Tunal → Portal Américas: **79.6 minutos**

## Cómo ejecutar el notebook
1. Abre el archivo `modelo_supervisado_transmilenio.ipynb` en Jupyter Notebook o VS Code.
2. Ejecuta las celdas en orden (primero las instalaciones, luego la generación del dataset y el resto del código).

**Nota:**  
Este proyecto demuestra la aplicación práctica de los conceptos del Capítulo 17, generando un modelo interpretable que complementa perfectamente el sistema basado en reglas y búsqueda heurística de la Actividad 2.