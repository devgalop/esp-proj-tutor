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

## Pasos para implementar un modelo de aprendizaje supervisado

1. **Recolección de datos**: Esta etapa implica la recopilación de un conjunto de datos etiquetado. Es importante asegurarse de que los datos sean representativos del problema que se desea resolver.

2. **Preprocesamiento de datos**: En esta etapa, se realizan tareas como la limpieza de datos, la normalización y la transformación de características para preparar los datos para el entrenamiento del modelo.

3. **División del dataset**: El conjunto de datos se divide en conjuntos de entrenamiento, validación y prueba para evaluar el rendimiento del modelo.

4. **Selección del modelo**: Se elige un algoritmo de aprendizaje supervisado adecuado para el problema que se desea resolver.

5. **Entrenamiento del modelo**: El modelo se entrena utilizando el conjunto de entrenamiento y se ajustan sus parámetros para minimizar el error.

6. **Evaluar el modelo con los datos de prueba**: Después de entrenar el modelo, se evalúa su rendimiento utilizando el conjunto de datos de prueba para medir su capacidad de generalización a nuevos datos.

7. **Despliegue y prediccion**: Finalmente, el modelo se despliega para hacer predicciones sobre nuevos datos en un entorno de producción.

## Algoritmos comunes en aprendizaje supervisado

Dentro del aprendizaje supervisado, existen varios algoritmos populares cada uno con sus propias características y aplicaciones. Algunos de los algoritmos más comunes son:

- **Regresión lineal**: Este algoritmo se utiliza para problemas de regresión donde su función principal es predecir el valor que continua. Se basa en la relación lineal entre las características de entrada y la etiqueta de salida. [leer más...](./LINEAR_REGRESSION.md)

- **Regresión logística**: Este algoritmo de clasificación se utiliza para predecir una variable binaria (por ejemplo, "sí" o "no"). Se basa en la función logística para modelar la probabilidad de que una instancia pertenezca a una clase específica.

- **Árboles de decisión**: Este algoritmo es una estructura tipo árbol, es utilizado para modelar decisiones y sus posibles consecuencias. Cada nodo del árbol representa una decisión mientras que las hojas representan las posibles etiquetas de salida.

- **Bosque aleatorio (Random Forest)**: Este algoritmo permite trabajar con multiples árboles de decisión para realizar predicciones más precisas. Cada árbol se entrena con una muestra aleatoria del conjunto de datos y las predicciones finales se basan en la mayoría de votos de los árboles individuales.

- **Máquinas de vectores de soporte (SVM)**: Este algoritmo se utiliza para crear un hiperplano que separa un espacio de n-dimensiones en clases distintas e identifica la categoría a la que pertenece cada instancia. Los casos extremos que ayudan a crear el hiperplano se llaman vectores de soporte.

- **K-vecinos más cercanos (KNN)**: Este algoritmo se basa en la idea de que las instancias similares tienden a estar cerca unas de otras. Para clasificar una nueva instancia, el algoritmo busca los k vecinos más cercanos en el espacio de características y asigna la etiqueta basada en la mayoría de votos de esos vecinos. El rendimiento de este algoritmo puede verse afectado por la elección de k y la escala de las características.

- **Gradient Boosting**: Este algoritmo combina clasificadores y árboles de decisión para crear un modelo más fuerte. Este método iterativamente ajusta los errores de los modelos anteriores para mejorar la precisión de las predicciones.

- **Naive Bayes**: Este algoritmo se basa en el teorema de Bayes y asume que las características son independientes entre sí. Es especialmente útil para problemas de clasificación de texto y spam.

| Algoritmo | Tipo de problema | Proposito | Método | Casos de uso |
| :--- | :---: | :---: | :---: | ---: |
| Regresión lineal        | Regresión         | Predecir valores continuos de salida         | Ecuación lineal que minimiza la suma de los cuadrados de los residuos | Predicción de valores continuos              |
| Regresión logística     | Clasificación     | Predecir variable de salida binaria          | Función logística que transforma la relación lineal                  | Tareas de clasificación binaria              |
| Árboles de decisión     | Ambos             | Modelar decisiones y resultados              | Estructura tipo árbol con decisiones y resultados                    | Tareas de clasificación y regresión          |
| Bosques aleatorios      | Ambos             | Mejorar la precisión en clasificación y regresión | Combinación de múltiples árboles de decisión                     | Reducir sobreajuste, mejorar precisión       |
| SVM                     | Ambos             | Crear hiperplano para clasificar o predecir valores continuos | Maximizar el margen entre clases o predecir valores continuos | Tareas de clasificación y regresión          |
| KNN                     | Ambos             | Predecir clase o valor basado en vecinos más cercanos | Buscar los k vecinos más cercanos y predecir por mayoría o promedio | Tareas de clasificación y regresión, sensible a datos ruidosos |
| Gradient Boosting       | Ambos             | Combinar modelos débiles para crear uno fuerte | Corregir errores iterativamente con nuevos modelos                  | Tareas de clasificación y regresión, mejorar precisión |
| Naive Bayes             | Clasificación     | Predecir clase basada en independencia de características | Teorema de Bayes suponiendo independencia de características | Clasificación de texto, filtrado de spam, análisis de sentimientos, médico |

La tabla de clasificación de algoritmos ha sido tomada de [GeeksforGeeks](https://www.geeksforgeeks.org/machine-learning/supervised-machine-learning/).

## Referencias

- [Introduction to Supervised Machine Learning](https://devblogs.microsoft.com/premier-developer/introduction-to-supervised-machine-learning/)
- [Supervised Machine Learning](https://www.geeksforgeeks.org/machine-learning/supervised-machine-learning/)
