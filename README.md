# Aplicacion-de-Interfaz-Grafica-de-Usuario---Analisis-Estadistico

## Descripción de la base de datos

La base de datos consiste en un conjunto de datos de informes de aerolíneas de Estados Unidos, la cual contiene aproximadamente 200 millones de reportes de vuelos nacionales de distintas aerolíneas reportados a la oficina de estadísticas de trasporte de los Estados Unidos. 

La base de datos contiene información básica sobre cada vuelo, tal como fecha, tiempo de vuelo, aeropuerto de salida, aeropuerto de llegada, etc. 

Este conjunto de datos está disponible en el Data Asset Exchange (DAX) de IBM en su plataforma web, en la que se proporcionan datos confiables y abiertos listos para usarse en aplicaciones para empresas. En específico esta base de datos cuenta con una licencia de permisos para usarla y modificarla. 

## Objetivos del proyecto y desarrollo

Supervisar e informar el rendimiento de los vuelos de las aerolíneas nacionales de EE.UU y de este modo analizar el desempeño de la aerolínea informante para mejorar su confiabilidad, mejorando así la confianza del cliente en la aerolínea. La interfaz cuenta con dos pestañas desplegables iniciales para seleccionar el tipo de reporte y el año del cual se desea el reporte:

![imagen](https://user-images.githubusercontent.com/43154438/135188611-fe06e213-a53d-4258-afbf-6edc1d368841.png)
#### Imagen 1: Vista inicial de la Interfaz de Usuario

El rango de años para los que el análisis se hizo fue entre 2005 y 2020.

Se creó una Interfaz Gráfica de Usuario (GUI) utilizando Plotly, el cual es un framework de Python para la construcción de aplicaciones analíticas web, y usando específicamente Dash, una librería de código abierto de Python para la construcción de Interfaces de Usuario. 

Dash es renderizada en navegadores web (renderiza componentes usando React.js), puede ser implementada en servidores y comunica paquetes JSON sobre consultas HTTP. Con esto es posible crear aplicaciones para responder cuestiones importantes de negocio. 

Dash posee componentes HTML para cada tag y atributo HTML por medio del cual se puede definir su estilo, diseño, disposición de la información, entre otros. También posee componentes core con el cual es posible darle interactividad a los elementos.

## Análisis y Resultados

Como se vio en la imagen 1, hay dos pestañas desplegables al iniciar la GUI, la primera es para seleccionar el tipo de reporte que se desea y cuenta con dos opciones: Informe Anual de Desempeño de la Aerolínea, y Estadísticas del Promedio Anual de Demoras de los Vuelos:

![imagen](https://user-images.githubusercontent.com/43154438/135188690-ec0ec012-90dd-4a76-b411-4889844a24a0.png)
#### Imagen 2: Primera pestaña desplegable

La segunda pestaña desplegable es para seleccionar el año del cual se desea el reporte. 

![imagen](https://user-images.githubusercontent.com/43154438/135188739-de2775de-feee-437e-a635-8797747e160d.png)
#### Imagen 3: segunda pestaña desplegable

Si se selecciona la primera opción de la pestaña desplegable y algún año se tendrán cinco gráficos en la ventana organizados gracias a los componentes HTML y core de la librería Dash de Plotly. Estos gráficos son:

-	Número de vuelos que vuelan a cada estado desde cada aerolínea informante utilizando el gráfico de mapa de árbol (Treemap-Chart).
-	Porcentaje de aterrizajes en aeropuertos desviados por aerolínea informante utilizando un gráfico circular (Pie-Chart).
-	Número de vuelos que vuelan desde cada estado utilizando Choroplet-Map (cuanto más sombreado un estado, más vuelos partieron de allí).
-	Tiempo medio de vuelo de la aerolínea informante mediante un gráfico de líneas (Line-Chart).
-	Número de vuelos en diferentes categorías de cancelación mediante gráfico de barras (Bar-Chart).

A continuación, se mostrará cada uno de estos cinco gráficos en su respectivo orden para el año 2020. Cabe aclarar que para el momento en que los datos fueron registrados, sólo habían transcurrido 3 meses del año 2020, por ende, sólo hay datos hasta el mes de marzo. A diferencia del resto de años donde se tienen datos por los 12 meses. 

![imagen](https://user-images.githubusercontent.com/43154438/135188798-f207c8c6-b46f-4610-957f-725f924f5896.png)
#### Imagen 4: Conteo de vuelos por aerolínea según Estado de destino representado en Treemap chart.

Acá cada recuadro grande representa un Estado y sus sub-recuadros son los Estados de Destino y podemos darnos cuenta de que en los estados FL (Florida) y TX (Texas) son las que más vuelos recibieron. Y en específico los Estados de Florida, Texas y Nueva York recibieron más vuelos de American Airlines.

Acá están escritos con abreviaciones de dos letras. Podemos pasar el mouse por cada recuadro y ver las estadísticas y números específicos por cada recuadro, así como acercarnos y ver cada aerolínea en detalle:

![imagen](https://user-images.githubusercontent.com/43154438/135188855-723021a7-cce5-4a13-808f-b8ee844e31cf.png)
#### Imagen 5: Estado FL (Florida) y representación gráfica de la cantidad de vuelos recibidos de cada Aerolínea: AA-DL-WIN, B6, etc.

![imagen](https://user-images.githubusercontent.com/43154438/135188876-c5d89d57-28fe-4d6d-9209-df94cf5bde87.png)
#### Imagen 6: Porcentaje de aterrizajes desviados dada la aerolínea

Podemos darnos cuenta de que sólo hubo un vuelo con aterrizaje desviado y es de la aerolínea YX (Midwest Express). A diferencia de otros años donde hubo más vuelos desviados y por parte de otras aerolíneas. 

![imagen](https://user-images.githubusercontent.com/43154438/135188914-297914f8-64bf-490c-8032-a32a06b4dd16.png)
#### Imagen 7: Número de vuelos desde cada estado en Choroplet-Map

Podemos darnos cuenta de que los Estados qué más vuelos enviaron son los estados de Texas, California, Georgia, Illinois y Carolina del Norte. Y si pasamos el mouse por encima de cada estado, podemos ver la cantidad específica de vuelos y la abreviatura del Estado de Origen.

![imagen](https://user-images.githubusercontent.com/43154438/135188954-9e6d03bf-c2a5-4920-a2ed-a4a5c5d99497.png)
#### Imagen 8: Cancelación de vuelos mensuales por mes según el código de cancelación en un bar-chart.

Podemos darnos cuenta de que solo durante los 3 primeros meses hubo cancelaciones de vuelo, donde durante los dos primeros meses hubo solo 3 cancelaciones por un mismo motivo (código de cancelación B), y hubo catorce cancelaciones de vuelo en el tercer mes, dos por el motivo A y doce por el motivo D.

![imagen](https://user-images.githubusercontent.com/43154438/135188991-73dd97c8-9911-4cfc-ab9a-726cbd632876.png)
#### Imagen 9: Promedio mensual de tiempo de vuelo por aerolínea en minutos en un Line Chart

Acá podemos ver por cada aerolínea la cantidad de minutos de vuelo acumulados en cada mes. Aquellas líneas que se ven incompletas son porque en un mes u otro no hubo vuelos por parte de esta. 

Pero si se quisiera ver con claridad el tiempo de vuelo de una aerolínea en específico y no confundirse con el resto, es posible eliminar temporalmente las otras dando click a las aerolíneas en la lista de la derecha del gráfico como se muestra a continuación:

![imagen](https://user-images.githubusercontent.com/43154438/135189031-5df84a20-d7fc-4ae2-be67-dba1f1586401.png)
#### Imagen 10: Promedio mensual de tiempo de vuelo en la aerolínea 9E (9-Air).

Podemos ver como en el primer mes su tiempo promedio de vuelo no supera la hora, mientras que en el segundo mes supera las dos horas, para caer el tercer mes a poco más de una hora promedio de vuelo. 

Por último, demos un vistazo a la disposición general de esta primera parte de la Aplicación de Interfaz Gráfica de Usuario que puede verse renderizada en un navegador web:

![imagen](https://user-images.githubusercontent.com/43154438/135189063-b234ece2-912c-4d81-ae5c-ce6be0f57045.png)
#### Imagen 11: Vista general de la disposición de los gráficos de la primera opción (Reporte Anual del Rendimiento de las Aerolineas).

Ahora bien, la segunda opción de reporte con los que cuenta la interfaz completa es el reporte de retardo anual de cada aerolínea el cual cuenta con cinco gráficos de línea que representa los retardos por mes de cada aerolínea. Existen diferentes motivos por el cual un vuelo se puede retardar, a continuación, se mostrarán cuatro de estos, además del tiempo de retardo promedio por cada uno.

Los cinco diferentes tipos de retardos graficados en esta sección de la interfaz son:

-	Retraso promedio mensual de la aerolínea informante para el año dado.
-	Retraso meteorológico promedio mensual por aerolínea informante para el año dado.
-	Retraso promedio mensual del sistema aéreo nacional según la aerolínea informante para el año dado.
-	Retraso de seguridad promedio mensual por aerolínea informante para el año dado.
-	Retraso promedio mensual de aeronaves tardías por aerolínea informante para el año dado.

A continuación, se muestran todos los cinco gráficos:

![imagen](https://user-images.githubusercontent.com/43154438/135189130-acb2e0d8-ea54-4493-ae00-1eef09c9be2e.png)
#### Imagen 12: Vista general de la disposición de los gráficos de la segunda opción (Reporte Anual de Retardos de Aerolíneas)

Estos Line chart cuentan con las mismas opciones y flexibilidades que el line chart de la primera opción que refleja el tiempo promedio de vuelo por aerolínea.

## Conclusiones

A través de una Aplicación de Interfaz de Usuario Web Interactiva es posible aclarar dudas sobre uno o varios aspectos clave de una empresa, negocio o proyecto mejor de lo que se podría hacer con los datos sin visualizaciones. Es agradable y práctico para el usuario y las partes interesadas en un negocio tener acceso a gráficos y visualizaciones que resuelvan una duda específica para de este modo planear una medida de mejora o un cambio útil.

Los científicos de datos pueden trabajar en colaboración con desarrolladores web para mejorar las funcionalidades de la página de una empresa por medio del uso de librerías como Dash y frameworks como plotly. Pero no solo para la mejora de una página web, sino, para construir aplicaciones personalizadas que permitan el análisis de diferentes aspectos del negocio, empresa o proyecto.  
