
 <h1 align="center">Proyecto-Individual-2-Data-Analitics-</h1>
 
 ![](https://laportadacanada.com/userfiles/images/accidentes-tragicos.jpg) 

 <h1 align="center">Accidentes-Aereos</h1>

Los accidentes aéreos son eventos inesperados e indeseados que involucran aeronaves y se producen daños físicos a personas o a la propia aeronave. Un accidente aéreo puede involucrar cualquier tipo de aeronave, incluyendo aviones comerciales, aviones privados, helicópteros, planeadores y globos aerostáticos.

Los accidentes aéreos pueden ser causados por diversos factores, como errores humanos, fallos de equipos, problemas meteorológicos, problemas de mantenimiento, fallas en la gestión del tráfico aéreo, problemas de diseño o problemas de fabricación. Y en cuanto a sus consecuencias, pueden ser tanto en términos de pérdidas humanas como económicas.

Es por eso que la industria de la aviación, las autoridades reguladoras y los investigadores trabajan incansablemente para mejorar la seguridad de la aviación y prevenir futuros accidentes. Por otro lado, para las organizaciones asociadas a la aviación, estudiar la causalidad de los accidentes y aprender a cómo prevenirlos en el futuro es clave para poder evitar pérdidas humanas y daños materiales significativos.

### Información del proyecto:
***
Organismo de la Organización de las Naciones Unidas, quiere investigar en profundidad los accidentes producidos desde inicios del siglo XX. Para ello, el objetivo principal es poder obtener un análisis de datos relacionado a esto, junto a un dashboard que complemente los análisis con sus visualizaciones.

Ya que el objetivo principal es poder obtener un análisis de los datos decidí encarar el proyecto con el fin de entender y poder llegar a una conclusión sobre 

### DICCIONARIO::open_book:

- Date - Fecha del accidente<br>
- Time - Hora local, en 24 h. en el formato hh:mm<br>
- Location - Ubicación del accidente<br>
- Operator - Aerolínea u operador de la aeronave<br>
- Flight -  Número de vuelo asignado por el operador de la aeronave<br>
- Route - Ruta completa o parcial volada antes del accidente<br>
- Type - Tipo de aeronave<br>
- Registration - Matrícula OACI de la aeronave<br>
- cn/In - Número de construcción o de serie / Número de línea o de fuselaje<br>
- Total Aboard - Total de personas a bordo<br>
- Passengers Aboard - Pasajeros a bordo<br>
- Crew Aboard - Tripulación a bordo<br>
- Total Fatalities - Muertes totales<br>
- Passengers Fatalities - Muertes de pasajeros<br>
- Crew Fatalities - Muertes de la tripulación<br>
- Ground - Total de muertos en el suelo, muertos por daño colateral<br>
- Summary - Breve descripción del accidente y la causa, si se conoce<br>

### Librerías Python utilizadas::books:
- Numpy 
- Pandas
- Matplotlib
- Seaborn
- Scipy
- Sklearn
  
### Objetivos del Trabajo:

Objetivo General:

"Analizar los accidentes de aviación ocurridos en los años especificados para comprender las causas subyacentes y las tendencias relacionadas con marcas de aeronaves, operadores, rutas y países."

Objetivos Específicos:

a. Identificar Causas de Accidentes:
"Identificar y categorizar las causas principales de los accidentes de aviación a partir de la información que se nos entrega en el dataset."

b. Analizar Marcas de Aeronaves:
"Determinar las marcas de aeronaves más frecuentemente involucradas en accidentes y analizar si hay patrones o tendencias en los tipos de aeronaves que sufren accidentes."

c. Evaluar Operadores:
"Identificar las aerolíneas u operadores con mayor incidencia de accidentes y analizar si existen factores comunes que puedan explicar esta tendencia."

d. Explorar Rutas de Vuelo:
"Analizar las rutas de vuelo para identificar las rutas que han experimentado un mayor número de accidentes."

e. Examinar Países Involucrados:
"Identificar los países en los que se produjeron la mayoría de los accidentes ."

f. Realizar Análisis de Correlaciones:
"Investigar posibles correlaciones entre diferentes variables, como marcas de aeronaves, operadores y tipos de accidentes, con el objetivo de descubrir patrones o relaciones significativas."

g. Generar Conclusiones y Recomendaciones:
"Elaborar conclusiones basadas en los análisis realizados y formular recomendaciones para mejorar la seguridad en la aviación, si es pertinente."

### Modelado de datos y transformación de los mismos:

En el archivo ETL se puede observar las transformaciones que se le realizaron al al dataset entre las cuales se pueden destacar:
- Se renombro algunas columnas para unificar el idioma.
- Se creo un diccionario.
- Se realizo cambio de dtype de algunas columnas.
- Varios datos que venían con el formato(?) se pasaron a datos nulos.
- Se trabajo en la columna Date para unificar las fechas a un mismo formato.
- De la columna Location se crearon otras dos para asi poder obtener Country y City por separado. 
- La columna Category se dividio en 2( Military y Passenger para poder tener una diferenciación de los vuelos.
- Se buscaron registros duplicados y faltantes.

### Realización del Análisis Exploratrorio(EDA)::bar_chart:

A los efectos de poder entender los datos presentados, se realizaron una serie de análisis y estudios sobre las variables del dataset a los efectos de poder encontrar relaciones entre los datos y comprender la relevancia de los mismos. Dentro de los análisis efectuados se encuentran:

- Distribuciones de frecuencias y estadísticas de las variables numéricas.
  
- Análisis e identificación de outliers en variables de interés (total_aboard y total_fatalities).
  
- Identificación de variables categóricas y sus valores.
  
- Gráficos de barras comparando las columnas.
  
- Gráficos de líneas realizando análisis temporales.



### Realización y obtención de los KPI'S:

Una vez realizado el Análisis Exploratorio y teniendo todo la informacón dispónibilizada se prosiguió al desarrollo del KPI sugerido en el trabajo y de uno prpuesto por nosotros:

- KPI 1:la tasa de fatalidad de la tripulación en los últimos 10 años, comparado a la década anterior. :pushpin:
  
Objetivo: Evaluar la disminución de un 10% la tasa de fatalidad.

Tasa de mortalidad de la tripulación: (Suma total de fallecidos en el período de tiempo / Suma total de accidentes en el período de tiempo)

- KPI 2:- 2do KPI:  Obtener la tasa anual de mortalidad de los accidentes registrados. :pushpin:

 Objetivo: reducir en un 5% la tasa, año a año.

Tasa Anual de Mortalidad = (Total Fatalities / All Aboard) * 100

### Dashboard: 

Para terminar con la presentación del análisis se realizo una presentación en Powerbi:

### Portada

![Logo](https://github.com/maga86/Data-Analist-Proyecto-2-Accidentes-Aereos/blob/main/src/Portada.png)

### Presentación

![Logo](https://github.com/maga86/Data-Analist-Proyecto-2-Accidentes-Aereos/blob/main/src/Presentaci%C3%B3n.png)

En la primer página se realizo  un resúmen de los objetivos a explorar y analizar que son los que nos van a ayudar no solo a entender el dataset si no tb encontrar las razones por las cuales los accidentes se pudieron haber dado:

-  Identificar Causas de Accidentes
-  Analizar Marcas de Aeronaves.
-  Evaluar Operadores.
-  Explorar Rutas de Vuelo.
-  Examinar Países Involucrados.
-  Realizar Análisis de Correlaciones.
-  Generar Conclusiones y Recomendaciones:

### KPI1:

![Logo](https://github.com/maga86/Data-Analist-Proyecto-2-Accidentes-Aereos/blob/main/src/KPI1.png)

En este kpi se debía obtener la tasa de mortalidad de la tripulación en los últimos 10 años.Presenta un gráfico central en el que se representa la tasa de mortalidad de la tripulación en los últimos 10 años. Tambien la acompaña un cuadro donde se puede visualizar mejor por década el valor de la mortalidad y para visualizar nuestro KPI tenemos una tarjeta que nos indica si se alcanzo la disminución de la mortalidad en un 10%. 

### KPI2:

![Logo](https://github.com/maga86/Data-Analist-Proyecto-2-Accidentes-Aereos/blob/main/src/KPI2.png)

En este kpi se debía obtener la tasa anual de mortalidad de los accidentes registrados y tiene como objetivo la reducción del 5% año a año.Se puede observar un gráfico central que muestra la mortalidad anual  traves del tiempo el cúal tambien interactua con las tarjetas de accidentes totales y muertes totales.
Por último podemos visualizar una tarjeta de KPI que muestra la tasa de mortalidad por año y su comparación con el target planteado (tasa del año anterior reducida en un 5% como mínimo). Si la tasa de mortalidad del año en cuestión es menor al target la tarjeta mostrará la tasa en color verde ( 2020). Caso contrario mostrará la tasa en rojo ( 2021). La tabla de análisis por año ayuda a clarificar sobre este KPI.


### Conclusiones:

A partir del desarrollo del EDA Y EL dashboard presentado se pueden obtener algunas conclusiones a tener en cuenta:

- Los vuelos que mas accidentes registran son lo vuelos militares con un 84% de registros frente a un 15% de los vuelo comerciales realizados.
  
- Estados Unidos, Rusia y Brasil son los países con mas registros de accidentes que hay ocupan los tres primeros puestos respectivamente.
  
- A la hora de analizar las rutas de vuelo aparecen con mas accidentes los vuelos llamados de entrenamiento "Training"y tambien entre los primeros puesto la ruta San Pablo- Río, Río-San Pablo. Quer condice con la información de Brasil en los primeros puesto de accidentes.
  
- Las marcas mas utilizadas por las aerolíneas son Douglas Company y Boing que asu vez son las que menos accidentes registran se podrían calificar como mas seguras que otras.

- La marca que mas accidentes presenta es el Douglas DC-3.

- En cuanto a los operadores  Aeroflot aparece como la que mas registros de muertes y tb de sobrevivientes. Al analizar u poco mas tambien se pudo ver que  Aeroflot es el operador con mayor cantidadde registros en este dataset.

- La tendencia anual de accidentes a lo largo de la historia comenzó una gran alza desde los días de los primeros vuelos hasta 1945. Esta tendencia pudo consolidarse entre 1946 y 2004 para finalmente romper la zona de acumulación en 2005 (año en que confirmamos la tendencia va hacia la baja comenzada en 1989).

- Podemos concluir que la aviación ha alcanzado un nivel de seguridad que  de accidentes más bajos de la historia, considerando la cantidad de vuelos, personas transportadas y avances tecnológicos.





