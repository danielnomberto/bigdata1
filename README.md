## AUTORES:

Carlos Daniel Nomberto Vela

## Objetivos
Realizar un análisis de sentimientos a un conjunto de datos provenientes de una red social (Instagram) en la cuenta de watson_fit. El objetivo es medir el nivel de aceptación o rechazo sobre su mensaje acerca de que "POCAS PERSONAS CUMPLEN SU PALABRA CON SÍ MISMAS... QUE EL DESARROLLO PERSONAL es CLAVE", entre otros temas que aborda en un podcast.

## Tecnologías utilizadas
- Procesamiento de datos: Pandas, Pyspark
- Análisis EDA: Pandas, Numpy, Matplotlib, Seaborn
- Lenguaje de programación: Python
- Otras librerías: NLTK, BERT
- Machine Learning: Scikit-learn
- Visualización: Matplotlib, Seaborn

## Comentario sobre el dataset
Se trata de un conjunto de datos en formato CSV obtenido de la página especificada, actualizado hasta el 12 de noviembre. Estos comentarios fueron descargados mediante la aplicación [exportcomments.com](https://es.exportcomments.com/) el 14 de noviembre, con un total de 130 registros.

## Hallazgos importantes
Durante el análisis, observamos que el consejo dado por el influencer es válido para su audiencia. Sería beneficioso profundizar más con datos como el género de la audiencia, horas de interacción, etc. Esto permitiría un enfoque más minucioso en estrategias de marketing.

## Conclusiones del proyecto
Se sugiere considerar el uso de un dataset más extenso o un modelo más potente para mejorar la precisión del modelo. Con la aplicación del modelo de regresión logística, se obtuvieron buenos resultados en la aplicación del análisis de sentimientos. Sin embargo, se requiere más información para perfeccionar el modelo.

## Herramientas y Librerías
```python
import pandas as pd
import numpy as np
import re
import time
import string
from sklearn import preprocessing, model_selection, naive_bayes, svm
from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
from sklearn.metrics import accuracy_score, confusion_matrix, classification_report
import matplotlib.pyplot as plt
import seaborn as sns
from nltk.sentiment.vader import SentimentIntensityAnalyzer
import nltk


