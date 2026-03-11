# Linear Regression Algorithm

La regresión lineal es un algoritmo de aprendizaje supervisado que asume una relación lineal entre las características de entrada y la etiqueta de salida. El objetivo de la regresión lineal es encontrar la mejor línea que se ajuste a los datos, minimizando la suma de los cuadrados de los residuos (diferencia entre los valores predichos y los valores reales).

Para la regresión lineal, se parte de la siguiente ecuación:

$$y=mx+b$$

donde:

- $y$ es el valor que se desea predecir
- $m$ es la pendiente de la recta
- $x$ es la variable independiente
- $b$ es la intersección con el eje $y$

En la regresión lineal se escribe la función de la siguiente manera:

$$y^ \prime = b + w_1x_1 + w_2x_2 + \dots + w_nx_n$$

donde:

- $y^ \prime$ es el valor predicho por el modelo
- $b$ es el término de sesgo o intersección con el eje $y$
- $w_i$ son los pesos asociados a cada característica $x_i$, estos pesos están asociados a la pendiente de la ecuación algebraica de la regresión lineal.
- $x_i$ son las características de entrada.

En el proceso de entrenamiento, se calculan los pesos $w_i$ y el término de sesgo $b$ utilizando un algoritmo de optimización, como el descenso de gradiente, para minimizar la función de pérdida, que generalmente es la suma de los cuadrados de los residuos.

## Métrica de Pérdida

La pérdida es una métrica utilizada para evaluar qué tan incorrectas son las predicciones del modelo. Esta se encarga de medir la diferencia entre los valores predichos por el modelo y los valores reales del conjunto de datos.

| Tipo de perdida | Definición | Ecuación |
| :--- | :---: | :---: |
| Perdida $L_1$ | Es la suma de los valores absolutos de la diferencia entre los valores predichos y los valores reales. | $\sum \left\|valor real - valor predicho\right\|$ |
| Perdida $L_2$ | Es la suma de los cuadrados de la diferencia entre los valores predichos y los valores reales. | $\sum \left(valor real - valor predicho\right)^2$ |
| Error absoluto medio (MAE) | Es el promedio de las perdidas $L_1$ en un conjunto de $N$ ejemplos. | $\frac{1}{n} \sum \left\|valor real - valor predicho\right\|$ |
| Error cuadrático medio (ECM) | Es el promedio de las perdidas $L_2$ en un conjunto de $N$ ejemplos. | $\frac{1}{n} \sum \left(valor real - valor predicho\right)^2$ |
| Raíz del error cuadrático medio (RECM) | Es la raíz cuadrada del error cuadrático medio (ECM). | $\sqrt{\frac{1}{n} \sum \left(valor real - valor predicho\right)^2}$ |

El MAE y el RECM pueden diferir bastante. El MAE representa el error de predicción promedio, mientras que el RECM representa la "dispersión" de los errores y se ve más afectado por los errores más grandes.

## ¿Cuándo seleccionar la regresión lineal?

El algoritmo de regresión lineal es una buena opción cuando se requiere predecir un valor númerico continuo. Sin embargo, es importante tener en cuenta estos aspectos antes de seleccionar este algoritmo:

- Los datos deben tener una relación lineal entre las características de entrada y la etiqueta de salida.
- No debe haber multicolinealidad entre las características de entrada, es decir, las características no deben estar altamente correlacionadas entre sí.
- El modelo de regresión lineal es sensible a los valores atípicos, por lo que es importante realizar un análisis de los datos para identificar y manejar los valores atípicos antes de entrenar el modelo.

## Referencias

- [Curso de regresión lineal de Google](https://developers.google.com/machine-learning/crash-course/linear-regression?hl=es-419)
- [Linear Regression](https://www.geeksforgeeks.org/machine-learning/ml-linear-regression/)
