## Working with real data

- Popular open data repositories:
  - UC Irvine Machine Learning Repository
  - Kaggle Datasets
  - Amazon AWS Datasets
- Meta portals
  - http://dataportals.org/
  - http://opendatamonitor.eu/
  - http://quandl.com/
- Otras paginas
  - Wikipedia list of Machine Learning Datasets

## Pipelines
Una sequencia de componentes de procesamiento de datos se llama **pipeline**.

## Select a Performance Measure
Una medida tipica para medir los problemas de regresion es **Root Mean Square Error (RMSE)**, da una idea de cuanto error hay en la prediccion.
**Root Mean Square Error**
$$
RMSE(X, h) = \sqrt{\frac{1}{m}\sum_{i = 1}^m (h(x^i) - y^i)^2}
$$

- **m** es el numero de instancias que hay en el dataset
- $x^i$ es el vector de todos los valores de caracteristicas excluyendo el label de la instancia i en el dataset.
- $y^i$ es la etiqueta
- $X$ es la matriz donde estan todos los valores de caracteristicas.
- $h$ es la funcion de prediccion del sistema, es llamada **hypothesis**
- $RMSE(X, h) es la funcion de costo medida en el set de ejemplos usando la hipotesis h.

Cuando existen muchos outliers dentro del dataset se puede usar **Mean Absolute Error**
$$
MAE(X, h) = \frac{1}{m}\sum_{i = 1}^m \lvert h(x^i) - y^i \rvert
$$

La norma $l_x$ de un vector **v** que contienen n elementos se puede definir como
$$
\lVert v \rVert = (\lvert v_0 \rvert^k + \lvert v_1 \rvert^k + ... + \lvert v_n \rvert^k)^\frac{1}{k}
$$

cuando es $l_0$ nos dice cuantos numeros diferentes a cero hay en el vector y si hacemos que tienda a infinito nos va a dar el valor absoluto maximo en el vector.

Cuando tenemos la norma $l_2$ es la distancia euclidiana desde el origen al punto

Cuando tenemos la norma $l_1$ se conoce como la distancia manhattan y es sumar por ejemplo en un vector de dos dimensiones la medida del eje x y del eje y