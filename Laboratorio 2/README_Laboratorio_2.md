# Laboratorio de Clasificación de Canciones de Spotify
Trabajos para la materia de Machine Learning de la UPSO

## Descripción
Este laboratorio, en el contexto de la asignatura de Machine Learning de la Universidad Provincial del Sudoeste (UPSO), se centra en el análisis de un conjunto de datos de canciones de Spotify. El objetivo es desarrollar un clasificador que, utilizando algoritmos de aprendizaje automático, pueda predecir si a un usuario le gustará o no una canción específica.

## Repositorio y Colab

Link al repositorio: [Laboratorio_2 Juan Manuel Roccia](https://github.com/JuanRoccia/MachineLearningUPSO/blob/main/Laboratorio%202/Laboratorio_Clasificador_Canciones_Spotify.ipynb)

Link al Colab: [Google Colab](https://colab.research.google.com/github/JuanRoccia/MachineLearningUPSO/blob/main/Laboratorio%202/Laboratorio_Clasificador_Canciones_Spotify.ipynb)

## Conjunto de Datos
El conjunto de datos proporcionado en formato CSV contiene 16 columnas, de las cuales 13 son atributos característicos de las canciones, además de las columnas para el nombre de la canción, el artista y la etiqueta "target" que indica las preferencias del usuario.

## Informe
El informe debe documentar el proceso de creación del programa clasificador, incluyendo la selección de características, entrenamiento de modelos, validación y ajuste de hiperparámetros. Cada paso debe estar justificado y explicado detalladamente.

## Desafíos y Soluciones
Durante el desarrollo del proyecto, surgieron varios desafíos, entre ellos:

1. **Selección de Características**: Determinar qué atributos del conjunto de datos eran más relevantes para la clasificación presentó dificultades iniciales. Se utilizó análisis de correlación y técnicas de selección de características para resolver esto.

2. **Desbalance de Clases**: Se observó un desbalance en las etiquetas de destino, lo que podría llevar a un sesgo en el modelo. Se aplicaron técnicas de sobremuestreo y submuestreo para mitigar este problema.

3. **Ajuste de Hiperparámetros**: La optimización de hiperparámetros fue un proceso intensivo en tiempo y recursos computacionales. Se emplearon métodos como Grid Search y Random Search para encontrar la mejor configuración.

4. **Evaluación de Modelos**: La interpretación de las métricas de rendimiento fue compleja debido a la naturaleza desbalanceada del conjunto de datos. Se puso especial atención en métricas como el recall y el F1-score, además de la precisión.

5. **Ensamble de Modelos**: La combinación de diferentes modelos para formar un ensamble presentó el desafío de elegir y ponderar adecuadamente cada modelo. Se optó por un enfoque de votación mayoritaria.

## Flujo de Trabajo
1. **Elegir Características Óptimas**: Se realizó un análisis de los atributos para seleccionar los más significativos.
2. **División en Entrenamiento y Prueba**: Se separaron los datos en conjuntos de entrenamiento y prueba para validar el rendimiento del modelo.
3. **Modelos de Machine Learning**: Se entrenaron varios modelos, incluyendo KNN, SVM, Árbol de Decisión y Naive Bayes.
4. **Validación**: Se aplicó validación cruzada k-fold para una evaluación más robusta.
5. **Ajuste de Hiperparámetros**: Se utilizó Grid Search y Random Search para optimizar los modelos.
6. **Ensamble de Modelos**: Se combinaron los modelos mediante votación mayoritaria.
7. **Evaluación del Rendimiento**: Se analizó el rendimiento utilizando la matriz de confusión, precisión, recall y F1-score.

## Contribución y Contacto
Este laboratorio es parte de un trabajo académico para la UPSO. Para consultas o colaboraciones, contactar a [juanroccia@gmail.com](mailto:juanroccia@gmail.com).
