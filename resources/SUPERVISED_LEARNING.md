# Supervised Learning - Machine Learning

El aprendizaje supervisado es un tipo de aprendizaje automático en el que el modelo se entrena utilizando un conjunto de datos etiquetado. En este enfoque, cada ejemplo de entrenamiento incluye tanto las características (inputs) como la etiqueta (output) correspondiente. El objetivo del modelo es aprender a predecir la etiqueta correcta para nuevos ejemplos basándose en las características aprendidas durante el entrenamiento.

El modelo genera predicciones utilizando las características de entrada y se compara con las etiquetas reales para calcular el error. El proceso de entrenamiento implica ajustar los parámetros del modelo para minimizar este error.

Los datos utilizados en el aprendizaje supervisado suelen tener una estructura clara en forma de matriz m x n donde m es el número de características y n el número de ejemplos. Cada fila representa un ejemplo de entrenamiento, mientras que cada columna representa una característica específica.

Dependiendo del tipo de dato de etiqueta, el aprendizaje supervisado se puede clasificar en dos categorías principales:

- **Clasificación**: Cuando las etiquetas son categorías discretas (por ejemplo, "spam" o "no spam"), el modelo se entrena para asignar cada ejemplo a una clase específica.

- **Regresión**: Cuando las etiquetas son valores continuos (por ejemplo, el precio de una casa), el modelo se entrena para predecir un valor numérico.

El aprendizaje supervisado se divide en tres etapas principales:

1. **Entrenamiento**: El modelo se entrena utilizando un conjunto del dataset inicial que contiene ejemplos etiquetados. El porcentaje de datos utilizados para el entrenamiento suele estar entre el 80% y el 90% del total del dataset.

2. **Validación**: Se utiliza un conjunto de datos diferente al de entrenamiento para evaluar el rendimiento del modelo y ajustar sus parámetros. Este conjunto de datos se conoce como conjunto de validación y suele representar entre el 10% y el 20% del total del dataset.

3. **Predicción**: Finalmente, el modelo se utiliza para hacer predicciones sobre nuevos datos que no han sido vistos durante el entrenamiento. Estas predicciones se basan en las características aprendidas por el modelo durante la fase de entrenamiento.

## Tipos de modelos de aprendizaje supervisado

## Referencias

- [Introduction to Supervised Machine Learning](https://devblogs.microsoft.com/premier-developer/introduction-to-supervised-machine-learning/)
- [Supervised Machine Learning](https://www.geeksforgeeks.org/machine-learning/supervised-machine-learning/)
