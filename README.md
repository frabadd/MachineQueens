## Autores:

- Julia de Enciso García (100533604)
- Paola León Tarife (100420266)
- Francisco Prados Abad (100542402)
- Camino Rodríguez Pérez-Carral (100445091)
- Paula Samper López (100541809)
- Lucía Yan Wu (100451764)

# Estudio Crediticio - Aprendizaje Automático

En este proyecto hemos realizado dos tareas:
- **Tarea de regresión**: predecir el valor de la variable continua ScoreRiesgo.
- **Tarea de clasificación**: predecir el valor de la variable binaria CreditoAprobado.
  
Se incluyen los siguientes notebooks y se recomienda el orden de lectura en el orden establecido:
- **1. `Preprocesamiento.ipynb`**: Preprocesamiento de los datos de `EstudioCrediticio_TrainP.csv`. 
- **2. `Regresion_modelos.ipynb`**: Modelos, resultados y conclusiones para la tarea de regresión.
- **3. `Clasificacion_modelos.ipynb`**: Modelos, resultados y conclusiones para la tarea de clasificación.

Asimismo, se incluyen las siguientes carpetas obtenidas tras el procesamiento de los datos:
- [`data/clasificación`](data/clasificación): incluye los archivos `X_train.csv`, `y_train.csv`, `X_test.csv`, `y_test.csv` obtenidos tras limpiar los datos para la tarea de clasificación.
- [`data/regresión`](data/regresión): incluye los archivos `X_train.csv`, `y_train.csv`, `X_test.csv`, `y_test.csv` obtenidos tras limpiar los datos para la tarea de regresión.
- [`encoders`](encoders): incluye el archivo `le.pkl` utilizado para transformar las columnas categóricas a numéricas.
- [`imputers`](imputers): incluye los archivos `imputer_cat.pkl` e `imputer_num.pkl` utilizados para reemplazar los valores nulos dependiendo del tipo de columna.
- [`scalers`](scalers): incluye los archivos utilizados para normalizar cada una de las columnas.
- [`models`](models): incluye los archivos  `modelo_clasificacion.h5` y `modelo_regresion.h5`, que contienen los mejores modelos obtenidos para cada tarea, es decir, los dos modelos de redes de neuronas de Keras enviados a la competición.

Por último, se recomienda instalar las librerías y dependencias necesarias para la ejecución del código, establecidas en `requirements.txt`.

# Resultados

Tanto para clasificación como para regresión, hemos obtenido los mejores resultados con redes de neuronas de Keras.

- Para regresión, el mejor MAE ha sido de 1.6282.
- Para clasificación, el mejor AUC ha sido de 0.9802.

Como trabajo futuro, podríamos mejorar la búsqueda de hiperparámetros para obtener mejores resultados.

La presentación de la defensa se puede encontrar en: [EstudioCrediticio-ML.pdf](EstudioCrediticio-ML.pdf)
