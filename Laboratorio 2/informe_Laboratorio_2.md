# Clasificador de Canciones de Spotify

Link al repositorio: [Laboratorio_2 Juan Manuel Roccia](https://github.com/JuanRoccia/MachineLearningUPSO/blob/main/Laboratorio%202/Laboratorio_Clasificador_Canciones_Spotify.ipynb)

## Introducción al Proyecto

### Contexto
Este proyecto surge con el objetivo de clasificar canciones de Spotify para predecir las preferencias musicales de los usuarios. Se ha utilizado un conjunto de datos con atributos significativos de diversas canciones para entrenar un modelo de aprendizaje automático, con la expectativa de que el rendimiento del modelo se alinee con nuestras hipótesis iniciales.

## Desafíos y Soluciones

### Preprocesamiento de Datos
El conjunto de datos fue examinado y preparado para el análisis sin valores faltantes. Se detectaron valores y se trataron características como 'instrumentalness', 'speechiness' y 'acousticness', ajustándolos para reflejar mejor la tendencia general de los datos, manejados mediante estrategias adecuadas manteniendo la integridad de los datos para el modelado predictivo.

### Selección de Características
Identificamos las características con mayor influencia en la preferencia de los usuarios, como 'danceability', 'speechiness' y 'instrumentalness'. Se eliminaron características irrelevantes y se trató la multicolinealidad para mejorar la precisión del modelo.

### Entrenamiento de Modelos
Seleccionar y configurar los modelos adecuados presentó dificultades. Experimentamos con varios modelos, incluyendo regresión logística y Gradient Boosting, y utilizamos Grid Search y Random Search para ajustar los hiperparámetros.

### Validación y Evaluación de Modelos
Utilizamos validación cruzada y analizamos las métricas de rendimiento para asegurar la fiabilidad de los modelos. Implementamos validación cruzada y analizamos meticulosamente las métricas de rendimiento para evaluar los modelos.

### Optimización de Hiperparámetros
Aplicamo la búsqueda del conjunto óptimo de hiperparámetros. El uso de Grid Search y Random Search ayudó a mejorar el rendimiento del modelo.

### Ensamblaje de Modelos
Combinar diferentes modelos para mejorar el rendimiento no fue trivial. El ensamblaje de modelos mediante votación mayoritaria mejoró los resultados finales.

### Interpretación de Resultados
Interpretar la matriz de confusión y otras métricas fue confuso en ocasiones. Ajustamos nuestros modelos y nuestra interpretación en respuesta a estos resultados.

### Computación y Tiempo
Optimizamos el uso de recursos computacionales para manejar la carga de trabajo eficientemente.

## Proceso de Desarrollo

### Preparación de Datos
Realizamos un análisis detallado para seleccionar las características más relevantes y preparamos los datos para el modelado. Se realizó un análisis de los datos para determinar qué información era relevante para el modelo, eliminando columnas innecesarias y experimentando con las características más relevantes.

### Modelos Considerados
Además de los modelos sugeridos inicialmente, consideramos:
- Regresión Logística
- Linear Support Vector Classification
- Light Gradient Boosting Machine
- Gradient Boosting Classifier

Estos modelos fueron seleccionados por su potencial para mejorar el rendimiento general y su eficiencia en tiempo de ejecución.

### Estrategia de Entrenamiento
Los modelos se entrenaron utilizando una división de datos estratégica y validación cruzada para garantizar una evaluación robusta.

 se han evaluado varios modelos de clasificación con el objetivo de identificar el que mejor se ajusta a los datos disponibles. Los resultados de precisión para cada modelo son los siguientes:

- KNN (K-Nearest Neighbors): 55.67% (+/- 4.45%)
- SVM (Support Vector Machines): 56.35% (+/- 2.79%)
- Decision Tree: 69.43% (+/- 5.12%)
- Naive Bayes: 61.56% (+/- 2.56%)
- Logistic Regression: 50.96% (+/- 0.23%)
- Linear SVC: 49.85% (+/- 1.91%)
- LGBM (Light Gradient Boosting Machine): 76.44% (+/- 3.54%)

Se observa que el modelo de Árbol de Decisión y LGBM superan significativamente a los demás modelos en términos de precisión. Sin embargo, es importante notar que el modelo SVM ha mostrado advertencias de no convergencia, lo que sugiere que se requiere un ajuste en el número de iteraciones o en los hiperparámetros para mejorar su rendimiento.

### Validación y Evaluación
Los modelos se validaron utilizando métricas de rendimiento estándar como precisión, recall, f1-score y la matriz de confusión. Estas métricas proporcionaron una visión detallada del rendimiento de cada modelo, permitiendo ajustes más informados durante la fase de evaluación.

### Ajuste de Hiperparámetros
El proceso de ajuste de hiperparámetros se llevó a cabo con cuidado, considerando un rango de valores para cada parámetro clave. Por ejemplo, se ajustaron el número de vecinos en KNN, el kernel y el margen de decisión en SVM, y la profundidad máxima y los criterios en el Árbol de Decisión. Los resultados de estas pruebas condujeron a una mejora significativa en la precisión y el rendimiento general de los modelos.

### Resultados Finales
Los resultados finales mostraron una mejora notable después del ajuste de hiperparámetros. El modelo GradientBoostingClassifier demostró ser el más eficaz, seguido de LGBM y luego de cerca por el Árbol de Decisión. 

Los resultados superaron las expectativas iniciales y confirmaron la efectividad de los métodos de ajuste empleados, así como la ventaja de combinar múltiples modelos para mejorar la precisión general.

## Reflexiones Finales

### Lecciones Aprendidas
A lo largo del proyecto, aprendimos la importancia de una evaluación meticulosa de los modelos y el ajuste de hiperparámetros. También se hizo evidente que la comprensión profunda de cada modelo y sus parámetros es crucial para el éxito del proyecto. Además, las advertencias de no convergencia en SVM resaltaron la necesidad de una configuración cuidadosa y la posibilidad de explorar modelos alternativos.

## Conclusión

Los desafíos enfrentados, como la no convergencia de SVM y la selección de hiperparámetros óptimos, fueron superados mediante un enfoque sistemático y la aplicación de prácticas de validación cruzada. Estos esfuerzos resultaron en un modelo robusto y confiable, cuya validez se refleja en las métricas de rendimiento mejoradas.

## Contacto

Para consultas o colaboraciones adicionales, por favor contactar a [juanroccia@gmail.com](mailto:juanroccia@gmail.com).
