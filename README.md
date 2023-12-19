# ProSalesAnalytics
Proyecto de Ciencia de datos para ayudar a una empresa a predecir las ventas y recomendar productos a sus clientes. 

El proyecto se basa en un primer modelo de series temporales con Random Forest Regression para predecir la cantidad de ventas de los productos para la siguiente semana.

Y el segundo modelo de Recomendación de productos con KNN Basic, utlizando la librería Surprise. Este modelo utiliza el filtrado colaborativo basado en clientes que sugiere productos a un usuario en función de las preferencias y comportamientos de usuarios similares.

![ProSales Analytics Logo](https://github.com/HellenEunice/ProSalesAnalytics/assets/145653265/96bc403e-625f-46c2-99ac-0f02a62ec017)

## Objetivo
- `Predecir las ventas semanales de los productos`. Crear un modelo sencillo que se adapte a la escasez de datos que luego sirva de base a la empresa para mejorar con el tiempo. 

- `Recomendar productos a clientes tomando cómo referencia las compras de clientes similares` Crear un modelo de recomendación sencillo que busque un patrón con clientes que compran productos similares para recomendarlo a otros. 

## Tecnologías Usadas
- `Lenguaje de programación:` Python
- `Bibliotecas:` Numpy, Pandas, Scikit-Learn, Surprise
- `Visualización de datos:` Matplotlib, Seaborn, Plotly Express
- `Modelos utilizados:` LinearRegression, Random Forest Regression, KNN, K Means

## Datos
La fuente de datos es una empresa real que vende productos de alimentación. A lo largo del proyecto se va a mantener algunos datos anonimos debido a la ley de protección de datos. Los datos disponibles son:

- Ventas de la empresa a lo largo de 20 semanas en sus diferentes canales de ventas.
- Productos disponibles en la tienda. 

## EDA

## Modelos
Para el proyecto se utilizaron varios modelos para lograr tres objetivos diferentes:
- Predicción de Ventas
- Recomendaciones de Productos a clientes
- Segmentación de clientes
  
### Predicción de Ventas
El modelo que mejor funciona para la cantidad de datos que teníamos es Random Forest Regression utilizando Series Temporales. 

## Otros Modelos para predicción de ventas. 
También utilizamos otros modelos de linear regression y random forest regression, utilizando nuevas variables creadas, pero no obtuvieron los mejores resultados. 
![Resultados de los modelos alternativos a series temporales](https://github.com/HellenEunice/ProSalesAnalytics/assets/145653265/4749fd42-5c33-4d33-bd4f-68153d2572c0)

# Conclusiones

## Cambios a futuro
