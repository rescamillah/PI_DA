# Proyecto individual Data analitics Henry
### Jovanni Escamilla

Descripcion del problema
Nos presentan una base de datos con la información de los siniestros víales en la Ciudad Autónoma de Buenos Aíres Argentina que ocurrieron en el año 2016 y hasta el 2021, esto con la intención de puder análizar los datos proporcionados y convertirlos en conocimiento, mismo que permita apoyar a la toma decisiones y ejercer medidas que ayuden a reducir el índice de homicidios derivados de estos siniestros.

Desempeño de funciones
Se nos pide asumir un rol de analista de datos, del cuál se desprende la encomienda de generar KPI's con la información proporcionada con la intención de generar políticas de rendimiento sobre los siniestros a futuro y su medición sobre la obtención de mejoras.

ETL
En la extracción inicial de la base de datos, nos damos cuenta que proviene de un archivo Excel, contenido con dos pestañas principales, llamadas "Homicidios" y "Víctimas", cada una de ellas cuenta con un diccionario de datos, el cuál nos indica el significado de cada una de las columnas y los valores encontrados en ellas.

Con la conclusión anterior, nos damos a la tarea de identificar los valores nulos y plasmarlos en cada uno de los valores de los registros existentes, verificando que no existieran registros duplicados y eliminando algunas columnas redudantes con información redundante, ya que la intención final de este apartado es la unión de ambas pestañas con una correcta definición del tipo de dato para cada una de las columnas mostradas en la base. 

Hay que tomar en cuenta que, en algunos de los registros donde se encontraron valores nulos, nos dimos a la tarea de hacer una exploración inicial de la información y realizando cierta investigación en páginas oficiales de internet, se lograron rescatar los valores correctos. 

Para mayor detalle, nos podemos referir al archivo ETL.ipynb, donde se encuentra cada uno de los pasos aplicados al dataset original, con la justificación que conlleva a realizar cada acción.

EDA
Ya con un archivo unificado, se procede a realizar el análisis y exploración de los datos, tomando en consideración aquellas columnas que sí resulten relevantes para la obtención de métricas funcionales para el proyecto y con la menor cantidad de valores nulos. 

A continuación, se enlistan las gráficas obtenidas en este análisis:
- Tendencia de siniestros por año
- Siniestros por comuna
- Siniestros por tipo de calle
- Siniestros por rol de víctima
- Siniestros por vehículo de la víctima
- Siniestros por vehículo del acusado

Para mayor detalle, nos podemos referir al archivo EDA.ipynb, donde se encuentra cada uno de los análisis aplicados a la base de datos, junto con una conclusión de cada una de las gráficas obtenidas, además, de que se presentan algunas propuestas de análisis que pueden valer la pena ser aplicados a futuro.

Dashboard
Para la implementación del dashboard se utiliza la herramienta de Power BI, la cuál se alimenta del archivo generado previamente en el notebook ETL.

Se comienza abordando la información de manera general, presentando la cantidad de siniestros que se han suscitado a lo largo del tiempo, además de la distribución de víctimas mortales que se presentaron en cada una de las comunas.
Con esta información podemos notar la tendencia de los siniestros y cuáles son las comunas que presentan un mayor número de muertes. 

Posteriormente, se presentan gráficas interactivos, donde se puede obtener información específica por año, comuna y edad de las víctimas, estos filtros pueden ser utilizados para análizar con mayor profundidad las gráficas propuestas que son:
- Siniestros por vehículo víctima: Donde se muestra el top 4 de los vehículos en los que viajaba la víctima
- Siniestros por vehículo acusado: En este gráfico, podemos ver el top 5 de los vehículos que son acusados de homicidio
- Distribución de siniestro por tipo de calle: Aquí analizamos cuáles son las principales vialidades en las cuáles se suscitan los siniestros
- Distrubución de siniestro por rol de víctima: Se presenta la distribución de muertes por el rol de la víctima.

Después, mostramos los 2 KPI solicitados más un KPI adicional en forma de propuesta para ser analizado:
1. Reducción de homicidios por semestre, de forma general se aborda el total de homicidios que se presentan en un semestre y se realiza su comparación contra el semestre anterior.
2. Reducción de homicidios a motociclistas, donde se busca que el número de víctimas que viajaban en motocicleta se vea reducido con respecto al año anterior.
3. Reducción de homicidios a peatones, se presenta esta propuesta con la intención de reducir el número de muertes a peatones que resultan ser víctimas de un siniestro vial.

Propuestas y Conclusiones
Por último, se presentan una seríe de conclusiones adicionales a las previamente analizadas en los gráficos interactivos, de las cuales se pueden desprender análisis a futuro sobre las víctimas de motociletas y peatones que a su vez, pudieran haber muerto a merced de autos o pasajeros. 

De igual forma, se plantea como propuesta realizar campañas de educación vial en dos vías:
1. Peatones, esto a raíz de notar que los peatones son una de las principales víctimas a lo largo del tiempo
2. Pasajeros, son estos uno de los principales roles acusados de cometer homicidio

Adicional, se habla sobre una propuesta con mayor detalle, en la que se analicen las avenidas y cruces en las que suceden con mayor frecuencia los siniestros, de tal forma que, se encuentren puntos estratégicos en dichas vialidades para incorporar algún semáforo, reductores de velocidad, señalizaciones, etc.
