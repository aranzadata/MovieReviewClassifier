# Movie_Review_Clasifier

Film Junky Union, una nueva comunidad vanguardista para los aficionados de las películas clásicas, está desarrollando un sistema para filtrar y categorizar reseñas de películas. El objetivo es entrenar un modelo para detectar las críticas negativas de forma automática. Para lograrlo, se utiliza un conjunto de datos de reseñas de películas de IMDB con leyendas de polaridad para construir un modelo para clasificar las reseñas positivas y negativas.

Se experimentó con tres tipos de clasificadores: Regresión Logística, Descenso de Gradiente y K Vecinos cercanos. Se utilizaron las librerías Nature Language Toolkit, spaCy para encontrar palabras vacías. También se observa el efecto de realizar lemmatización. Para cada una de estas opciones se realiza una bolsa de palabras y vectorización con IF_IDF.

De todos los modelos se encontró que el de Regresión Logística con librería NLTK y sin lematización fue el que mejores resultados obtuvo, con un score f1 en el conjunto de prueba de 0.88. Este mismo modelo con la librería spaCy y con lemmatización no mejoró significativamente los resultados.

Por otro lado el clasificador con Descenso de Gradiente obtuvo las segundas mejores métricas, y estas probablemente pueden mejorar haciendo una búsqueda de hiperparámetros. Nuevamente la lematización no mejoró significativamente las métricas.

Para el clasificador de K Vecinos Cercanos se realizó una búsqueda de parámetros para el número de vecinos cercanos. Las predicciones para este modelo tuvieron menor exactitud, pero mostraron la mejor consistencia.
