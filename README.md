# OilyGiant_Oil
OilyGiant Oil Extraction Company - Predicting the volume of reserves and maximizing expected profits

En este proyecto vamos a trabajar con los datos de la compañía de extracción de petróleo OilyGiant. 

Nuestra tarea es encontrar los mejores lugares donde abrir 200 pozos nuevos de petróleo.

Tenemos los datos sobre muestras de crudo de tres regiones. Debemos crear un modelo que ayude a elegir la región con el mayor margen de beneficio. Además de analizar los beneficios y riesgos potenciales utilizando la técnica bootstrapping.

Librerías Utilizadas:

las librerías que ocuparemos en el proyecto:

  - import pandas as pd # importamos las librerías de pandas
  - from matplotlib import pyplot as plt # importamos las librerías pyplot de Matplotlib
  - import numpy as np # importamos la librerías de NumPy, se usa para funciones matemáticas complejas
  - from scipy import stats as st # importamos el módulo stats de la librería SciPy.
  - import seaborn as sns # importamos la librería Seaborn para realizar unos gráficos
  - sns.set_theme() # ocupamos esa librería para tener meejores gráficos
  - from sklearn.model_selection import train_test_split #importamos la función train_test_split biblioteca scikit-learn
  - from sklearn.utils import shuffle # importamos la función shuffle de la biblioteca scikit-learn
  - from sklearn.linear_model import LinearRegression
  - from sklearn.metrics import mean_squared_error

En este proyecto trabajamos con 3 conjuntos de datos de la compañía de extracción de petróleo OilyGiant. El objetivo era de determinar la mejor región donde abrir 200 pozos nuevos de petróleo. 

Para ello, después de descargar los datos, hemos ocupado un modelo de regresión lineal, con el cual hemos analizado las posibles ganancias en cada una de las regiones, ocupando para ello los 200 pozos con los valores de predicción más altos de cada una de las 3 regiones. 

Basándonos sólo en ese análisis de ganancias potenciales, la Región 0 parece ser la opción más atractiva para el desarrollo de pozos petrolíferos, debido a que proporciona una ganancia potencial mayor que las otras dos regiones.

Posterior a eso hemos ocupado técnica del bootstrapping con 1000 muestras, calcular el beneficio promedio, el intervalo de confianza del 95% y el riesgo de pérdidas.
