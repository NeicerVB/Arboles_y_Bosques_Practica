# **Prácticas de Árboles de Decisión y Bosques aleatorios**

# **Ingresos del censo**
Este proyecto pretende aplicar dos modelos basados en árboles de decisión y bosques aleatorios para predecir si una persona gana más de 50.000 dólares al año. El dataset utilizado será de la página web de la UCI <a href="https://archive.ics.uci.edu/dataset/20/census+income">Ingresos del censo</a> y cuenta con 48.842 filas y 14 columnas.
<div style='text-align: center;'>
    <img src="https://cdn-icons-png.flaticon.com/128/16136/16136294.png" alt='Ingresos'>
</div>

## Objetivo 🛣️
El objetivo es clasificar a las personas en dos categorías: si ganan más de 50.000 dólares al año o no. Se esperan que los modelos puedan darnos información clara cuando deseamos conocer cuales son las características que influyen en la clasificación de las personas.

## Metodología 💡
1. **Inspección y Limpieza**: Conocer los tipos de datos, la cantidad de valores nulos y la distribución de las variables.
2. **EDA**: Exploración de valores nulos, análisis univariado y bivariado, análisis de correlación y detección de outliers. Además, se prevee aplicar imputación o eliminación de valores nulos y codificación de variables categóricas.
3. **Reducción de dimensionalidad**: Se aplicará PCA para reducir la dimensionalidad del dataset.
4. **División de datos**: Se dividirán los datos en conjuntos de entrenamiento y prueba en una proporción de 75:25.
5. **Modelado**: Se utilizarán las clases `DecisionTreeClassifier` y `RandomForestClassifier` provenientes de la librería de scikit-learn.
6. **Evaluación**: Se evaluará el modelo considerando principalmente la métrica de f1_weighted, debido a que el dataset se encuentra desbalanceado y se desea darle más peso a la clase minoritaria.