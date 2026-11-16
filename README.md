# Proyecto 2 - Procesamiento de imágenes y Regresión Lineal Múltiple

## Descripción

Este proyecto tiene como objetivo aplicar herramientas de Python para trabajar con datos y desarrollar un modelo de aprendizaje automático.

En la segunda parte del proyecto se implementó un modelo de **Regresión Lineal Múltiple** para estimar el precio de propiedades utilizando información relacionada con sus características y ubicación.

## Herramientas utilizadas

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- ucimlrepo

## Dataset

Se utilizó el conjunto de datos **Real Estate Valuation**, obtenido del repositorio UCI Machine Learning Repository.

El dataset contiene 414 registros de propiedades y distintas variables relacionadas con su ubicación y características.

Fuente: https://archive.ics.uci.edu/dataset/477/real+estate+valuation+data+set

## Desarrollo del modelo

Se seleccionaron cinco variables predictoras:

- Antigüedad de la propiedad.
- Distancia a la estación de MRT más cercana.
- Cantidad de comercios cercanos.
- Latitud.
- Longitud.

La variable objetivo fue el precio por unidad de superficie.

Los datos se dividieron en un 80 % para entrenamiento y un 20 % para prueba. Luego se entrenó un modelo de Regresión Lineal Múltiple y se evaluó su rendimiento utilizando las métricas R², MSE y RMSE.

## Resultados obtenidos

| Métrica | Entrenamiento | Prueba |
|---|---:|---:|
| R² | 0,546 | 0,675 |
| MSE | 85,433 | 54,581 |
| RMSE | 9,243 | 7,388 |

La variable con mayor influencia relativa, según los coeficientes estandarizados, fue la distancia a la estación de MRT, con un coeficiente de -0,404.

## Conclusiones

El modelo logró explicar aproximadamente el 67,5 % de la variabilidad de los precios en el conjunto de prueba. Los resultados muestran que las variables seleccionadas aportan información útil para realizar estimaciones.

La distancia al transporte público fue la variable con mayor influencia relativa y presentó una relación negativa con el precio. También se observó una relación negativa con la antigüedad de la propiedad y positiva con la cantidad de comercios cercanos.

Si bien el modelo obtuvo resultados razonables, sería posible mejorar su capacidad predictiva incorporando otras características, como la superficie, el estado de conservación y la cantidad de habitaciones de cada propiedad.

## Archivo del proyecto

El desarrollo y la ejecución del modelo se encuentran en el siguiente notebook:

`Proyecto2_Regresion_Lineal_Multiple_Azcarate_Ferreyra.ipynb`
