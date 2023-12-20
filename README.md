# ProSalesAnalytics
Proyecto de Ciencia de datos para ayudar a una empresa a predecir las ventas y recomendar productos a sus clientes. 

El proyecto se basa en un primer modelo de series temporales con Random Forest Regression para predecir la cantidad de ventas de los productos para la siguiente semana.

Y un segundo modelo de Recomendación de productos con KNN Basic, utlizando la librería Surprise. Este modelo utiliza el filtrado colaborativo basado en clientes que sugiere productos a un usuario en función de las preferencias y comportamientos de usuarios similares.

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
La fuente de datos es una empresa real que vende productos de alimentación. A lo largo del proyecto se va a mantener algunos datos anóninimos debido a la ley de protección de datos. Los datos disponibles son:

- Ventas de la empresa a lo largo de 20 semanas en sus diferentes canales de ventas.
- Productos disponibles en la tienda. 

## EDA
El análisis exploratorio de datos lo realizamos teniendo cómo base los clientes, ventas y productos, para ver cómo influían las diferentes variables en ellos.

![EDA de comparación de clientes que más comprán con los clientes que más visitan la tienda](https://github.com/HellenEunice/ProSalesAnalytics/assets/145653265/55fc8c6f-85fe-4f4d-95c5-8bb87ea73f64)

![EDA sobre las ventas totales según canal de venta y mes](https://github.com/HellenEunice/ProSalesAnalytics/assets/145653265/1cb8df29-f77d-4f4f-9f71-738f0d2038bc)

![EDA sobre la evolución de ventas de las categorías en los meses](https://github.com/HellenEunice/ProSalesAnalytics/assets/145653265/3e0adedf-7c3a-408d-89ee-67521f11a421)


## Modelos
Para el proyecto se utilizaron varios modelos para lograr tres objetivos diferentes:
- Predicción de Ventas
- Recomendaciones de Productos a clientes
- Segmentación de clientes
  
### Predicción de Ventas
El modelo que mejor funciona para la cantidad de datos que teníamos es Random Forest Regression utilizando Series Temporales con un RMSE de 0.7144
y R2 de 0.3195. 

![Gráfico sobre el resultado del modelo de Series Temporales ](https://github.com/HellenEunice/ProSalesAnalytics/assets/145653265/51cf99ab-febf-46d3-b68e-d3a6abe0f280)


### Otros Modelos para predicción de ventas. 
También utilizamos otros modelos de linear regression y random forest regression, utilizando nuevas variables creadas, pero no obtuvieron los mejores resultados. 
![Resultados de los modelos alternativos a series temporales](https://github.com/HellenEunice/ProSalesAnalytics/assets/145653265/4749fd42-5c33-4d33-bd4f-68153d2572c0)


### Recomendación de Productos
Para la recomendación de productos utilizamos la librería Surprise y el modelo KNN Basic, que obtuvo un error de RMSE de 24.0376 y R2 de 0.3177. 
![Resultado del modelo de recomendacion de productos](https://github.com/HellenEunice/ProSalesAnalytics/assets/145653265/94feda14-c6d3-4e19-9cdc-2ffe636bceba)


### Segmentación de clientes
Hemos intentado segmentar los clientes en grupos homogéneos según comportamientos de compra y preferencias con el modelo de aprendizaje no supervisado K-means.
![Resultado del modelo de segmentación de clientes](https://github.com/HellenEunice/ProSalesAnalytics/assets/145653265/f282f901-ee3a-46f2-94e0-6e7c63db2625)


# Conclusiones
- Dado a la escasez de datos, los modelo no dan el resultado óptimo.
- El proyecto sienta las bases para futuras mejoras con la incorporación de más datos y técnicas avanzadas. La implementación efectiva de estos resultados puede llevar a la optimización continua y al crecimiento sostenible de la empresa.


## Cambios a futuro
- Aumentar la cantidad de datos y variables que ayuden a comprender mejor las ventas y los clientes.
- Con el aumento de datos, se puede probar con modelos más avanzados. 

