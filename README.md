# PROYECTO 6: SISTEMA DE RECOMENDACIÓN
En este proyecto se construye un sistema de recomendación de películas utilizando la librería Surprise para su creación y análisis. Se trabaja sobre el dataset de versión 100k de [MovieLens](https://grouplens.org/datasets/movielens/) el cual se basa en un sistema de rating de cinco estrellas y texto libre para tags. Contiene 100.000 ratings para 1.682 películas con datos creados por 943 usuarios, los cuales calificaron al menos 20 películas cada uno. Además, se emplean otras librerías como MatPLotLib, Numpy y Collections.

El procedimiento utilizado se menciona a continuación:
-	Descripción de los datos.
-	importación de Reader desde Surprise y configuración de los parámetros 'line_format' igual a 'user item rating timestamp' y 'sep' igual a '\t' para poder leer la información.
-	 Ejecución inicial de Cross Validation y el algoritmo SVD e impresión de resultados de los RMSE de testing.
-	Evaluación del RMSE promedio resultante del Cross Validation sobre el conjunto de testing de acuerdo a la cantidad de factores en SVD y visualización grafica de estos con MatPotLib.pyplot.
-	Con GridSearchCV, se encuentra el mejor estimador SVD con 500 factores, para un espacio de parámetros definido, se imprime el mejor RMSE y se obtiene el mejor estimador ya ajustado como resultado.
-	Se obtiene una predicción para un conjunto de datos especifico.
-	Desarrollo de una función para una situación específica de recomendación y se prueba el modelo.
