<div align="center">
  
# Modelos de Clasificación: Alfarería Romano-Británica
<p>
  <img src="imagenes/intro.png" width="500">
</p>
<br> 

</div>

# Resumen del Proyecto

El proyecto se centra en la aplicación de modelos de clasificación a las muestras de una antigua alfarería Romano-británica, recolectadas de cuatro sitios en el Reino Unido (L, C, I, A), a las cuales se les realizó un análisis químico detallado para medir el porcentaje de cinco óxidos metálicos presentes en cada muestra: Aluminio (Al), Hierro (Fe), Magnesio (Mg), Calcio (Ca) y Sodio (Na).

# Objetivo

Predecir el sitio de origen de las muestras en función de su composición química, utilizando diferentes modelos de clasificación. 

# Tecnologías Utilizadas

* Lenguaje  : Python
* Librerías : ´pandas´, ´numpy´, ´matplotlib´, ´seaborn´, ´scikit-learn´, ´sklearn´
* Entorno   : Visual Studio Code

# Descripción de los Datos

El conjunto de variables predictoras corresponde a los siguientes químicos encontrados en las muestras de alfarería Romano-británica: 

- **Aluminio (Al)** : Porcentaje de aluminio en la muestra.
- **Hierro (Fe)**   : Porcentaje de hierro en la muestra.
- **Magnesio (Mg)** : Porcentaje de magnesio en la muestra.
- **Calcio (Ca)**   : Porcentaje de calcio en la muestra.
- **Sodio (Na)**    : Porcentaje de sodio en la muestra.

La variable objetivo esta dada por **Sitio**, la cual representa el lugar de origen de la muestra. Esta variable es categórica, teniendo como posibles alternativas: *C, I, A y L*.


# Procedimiento

* Análisis exploratorio de los datos
* Procesos de extracción y limpieza de datos
* Análisis de pertinencia de Annova
* Implementación de modelos de Machine Learning: Decision Trees y Random Forest.

# Resultados

Se implementaron dos modelos de clasificación, cada uno con resultados destacados:

* **Análisis ANOVA:** Se realizó un test ANOVA para evaluar la independencia, la normalidad de las observaciones y la homocedasticidad entre grupos. Sin embargo, no se cumplieron las condiciones de normalidad para todo el conjunto de datos, lo que llevó a la conclusión de que no correspondía realizar un test ANOVA en este contexto.

* **Decision Tree Classifier:** Este modelo inicial logró un accuracy *(porcentaje de predicciones correctas sobre el total de predicciones realizadas)* del **75%**. Se realizó un análisis de errores a través de una matriz de confusión, permitiendo identificar las predicciones incorrectas y mejorar el modelo.

* **Random Forest Classifier:** Con una búsqueda de hiperparámetros mediante grid search, este modelo alcanzó un accuracy del **87.5%**, superando notablemente al modelo anterior.

# Conclusiones

A través de la aplicación de técnicas de machine learning, este proyecto demuestra la utilidad de los métodos de clasificación en el análisis químico de la alfarería. Además, en este contexto, la capacidad de predecir el sitio de origen de las muestras en función de su composición química no solo contribuye al entendimiento histórico de la alfarería Romano-británica, sino que también muestra el potencial de la ciencia de datos en el análisis arqueológico. Estos resultados subrayan la importancia de seleccionar el modelo adecuado y optimizar sus parámetros para obtener una clasificación más precisa.
