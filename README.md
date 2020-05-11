# PAP ITESO 2020
## PROGRAMA DE MODELACION MATEMATICA PARA EL DESARROLLO DE PLANES Y PROYECTOS DE NEGOCIO I
### CENACE: Pronósticos de generación de plantas intermitentes
### Flores Orozco, Oscar Alfonso; Ramírez Cambero, Job; González Juárez, Edgar Ranulfo

***

### OBJETIVO GENERAL: 

* Generar un modelo para el pronóstico de variables horarias, usando datos de generación de energía proveídos por el CENACE.
* Se utilizarán modelos autorregresivos como ARIMA y modelos dinámicos de regresión hacer las predicciones y se hará una diferenciación entre plantas solares y eólicas, por que su comportamiento es distinto.
* Pondremos a competir los modelos creados, para obtener un menor tiempo de corrida con mayor eficiencia.

***

### OBJETIVOS ESPECÍFICOS:

* Obtener datos históricos:
  * Plantas solares (fotovoltaicas)
    * energía (MWh)
    * radiación solar (kW/m2)
    * temperatura (°C)
    * nubosidad (%)
    * humedad relativa (%)
    * velocidad del viento (km/h)
    * presión barométrica (mbar)
    * radiación indirecta (kW/m2)
  * Plantas eólicas (aerogeneradores)
    * energía (MWh)
    * velocidad del viento (km/h)
    * dirección del viento (la referencia será el norte)
    * temperatura (°C)
    * nubosidad (%)
    * humedad relativa (%)
    * presión barométrica (mbar)
* Filtrar y ordernar la información obtenida
* Obtener un modelo para el pronóstico de las variables
* Probar el modelo obtenido y obtener sus estadísticos

***

### METODOLOGÍA DE TRABAJO:

* Herramientas a utilizar 
    * Excel 
    * Python
    * Jupyter notebook 
* Plataforma para sincronicar
    * GitHub
    * GitKraken
* Librerías a considerar
    * Pandas
    * Numpy 
    * Pmarima
    * Statsmodels
* Criterios a contemplar 
    * MAPE y MAE < 10%
    * Tiempo de ejecución > 10 minutos
* Meta a lograr
    * Modelos ARIMA o dinámicos para la predicción de generacion en las plantas intermitentes tanto solares, como eólicas. 

***

### AVANCES 

#### Bloque 1 (Presentación) 

20 de enero de 2020 – 1 de febrero de 2020

Se definieron objetivos generales del PAP los cuales fueron mencionados previamente en el resumen. Se observó cómo los equipos del semestre pasado trabajaron y algunos ejemplos que compañeros que ya trabajaron previamente en el PAP, entregaron. Se dejó como objetivo que cada código en Python del equipo anterior se debe de correr en un tiempo menor a 10 minutos como límite, aunque lo mejor será en un tiempo de aproximadamente 5 minutos o menor, aunque no se definió el lenguaje a usar a lo largo de las prácticas.
Además, se destacó que existen dos modelos que serán usados durante el PAP: Modelos Explicativos (D = T + E + …) y los Modelos de Series de Tiempo (x_t= x_(t-1)+x_(t-2)+⋯). Se acordó también que se van a hacer visitas periódicas al CENACE para obtener retroalimentación por parte de ellos y comparar los resultados obtenidos. Algunos otros entregables son: RPAP, el reporte de las prácticas que incluye las bitácoras, juntas periódicas para ir mostrando avances y la presentación final de los resultados.  Al final, se compartió lo que se realizó el semestre pasado por algunos alumnos, para analizarlo y revisar la información y datos que puedan ser útiles para comenzar. 
Para tener un desempeño óptimo de las actividades, se integró un equipo de trabajo de dos a tres personas. Además de esto, se consultó con Pablo Benavides la forma de llevar a cabo cada proyecto para no tener errores que resulten de la falta de comunicación. Se tuvo la primera reunión con el CENACE, en la cual Camilo Narváez compartió la forma en la que el CENACE trabaja y se desarrolla, dio a conocer los problemas por atacar este semestre, sus objetivos y lo que se busca lograr con el Proyecto de Aplicación Profesional en cuestión.

#### Bloque 2 (Entendimiento)

3 de febrero de 2020 – 15 de febrero de 2020

Se realizó la segunda reunión con el CENACE, ahora con el equipo y la gerencia de desarrollo de aplicaciones, en la cual se definió el método de comunicación para que se les hagan llegar los resultados y los programas que se estén desarrollando durante el periodo de colaboración.
Se definieron cuáles serían las herramientas que se utilizarían (Excel, Python, Jupyter, GitHub y GitKraken) y un dato a destacar es que todos se pueden utilizar de forma remota, lo que facilita trabajar a cualquier hora independientemente de la disponibilidad de cada integrante. Las carpetas se entrelazaron y compartieron para poder trabajar cada uno desde su ordenador y se cargó el código implementado por el equipo anterior.
Se inició definiendo cada problema que el CENACE hizo llegar y se terminaron de definir los equipos de trabajos. Cada problema tiene que ser probado con el MAE (Mean Absolute Error) y MAPE (Mean Absolute Percentage Error), donde el resultado de cada uno debería quedar debajo del 20%. El problema será el Pronóstico de Generación de Plantas Intermitentes.  
Los objetivos para la siguiente semana son: cargar código en GitHub, pronóstico 1 año completo o MAE < 20% o MAPE < 20%, estadística descriptiva de los resultados, Pull Request, ediciones, mejoras o propuesta de reestructuración completa del código.  
Se comenzaron a buscar APIs para bajar los datos históricos del clima, la desventaja fue que se tenían que estar bajando los datos de un Excel, y los datos eran de cada tres horas y no cada hora, esta propuesta del clima fue rápidamente cambiada y cambiamos el foco de atención. 

#### Bloque 3 (Desarrollo)

17 de febrero de 2020 – 29 de febrero de 2020

Se le dio prioridad a tratar de comprender el código que el semestre pasado otras personas realizaron sobre la generación de plantas intermitentes. Además, se dejó la tarea de realizar la presentación para el CENACE con los objetivos (general y específico), metodología y avances en el proyecto, próximamente en el transcurso de la semana se irá a presentar.
Se desarrolló un ensayo de presentaciones, como si ya fuera la exposición ante el CENACE, únicamente con los integrantes del equipo, lo que ayudó a tener retroalimentación y poder hacer mejoras antes de presentarla la siguiente semana ante el CENACE. En este ensayo se explicó objetivo general del proyecto, objetivos específicos, metodología del trabajo y fechas para los futuros avances. 
Se detectaron problemas en el código, por lo tanto, el enfoque durante el bloque 3 fue resolverlos. Había librerías especiales que no se estaban considerando y se tuvieron que implementar para poder correr el código de manera correcta. Después de notar que el código solo podía correr con ciertos días, se solucionó el problema y pudo correrse con cualquier día. Otro problema que se encontró fue que se reciclaban algunos datos y también se logró encontrar una solución. Además, se siguió mejorando el algoritmo que ya existía, sin embargo, arrojó el mismo error que al equipo pasado en la planta número 12.

#### Bloque 4 (Optimización)

2 de marzo de 2020 – 14 de marzo de 2020 

Se hizo la presentación de objetivos ante el CENACE, junto con una muestra de los primeros avances. Se hizo un acuerdo de entregar un archivo por planta de generación, para que ellos puedan elegir cuál quieren observar, y no un ciclo con todas las plantas, lo cual se puede alentar al momento de estar realizando el código. Además, se va a realizar dos veces, una separando las plantas por hora, y otro dejando la planta como una sola serie de tiempo, esto con el fin de encontrar cuál presenta mejores resultados. Solucionando el problema de solo poderlo correr en ciertos días, se podía hacer un análisis de días variables.

#### Bloque 5 (Implementación)

16 de marzo de 2020 – 28 de marzo de 2020

La suspensión de actividades debido al Covid-19 cambió un poco los planes. Se hizo la separación en By plants by hour donde se separa por hora cada planta y se trabajan 24 modelos (como su nombre lo dice, un modelo por hora) y By plants not by hour (donde la planta es tomada como una sola serie de tiempo) y se identificó que no había mucha diferencia, y que se podría trabajar con las plantas de generación como una sola serie por planta.
Después de realizar la separación de los datos y concluir que se trabajará con una sola serie por planta, se efectuó un análisis de esas series, donde se graficaron las primeras y segundas diferenciaciones de las series, para analizar la forma en la que se comportaba su autocorrelación, todo esto con el fin de nosotros encontrar el modelo óptimo de predicción de la generación de energía. Después, se busca el valor de p y q correspondientes. Además, se realiza la prueba de Dickey-Fuhller, para conocer si la serie es o no estacionaria.

#### Bloque 6 (Desarrollo)

30 de marzo de 2020 – 18 de abril de 2020 

En este bloque se cruza Semana Santa. En esta semana se le presentaron a Pablo los avances del trabajo mediante Microsoft Teams, sus comentarios sobre ellos fueron que positivos, mencionando que va muy bien y que siguiéramos con las pruebas de los modelos ARIMA, con los valores de p, d y q que se encontraran de las gráficas y así fue como se resolvió; se realizaron algunas pruebas con diferentes valores para encontrar el modelo con menor error absoluto, obteniendo de momento, un modelo ARIMA (8,1,2) con error de 25%. En otra sesión online se expuso un avance de los resultados obtenidos hasta el momento a CENACE. Faltaría probar el modelo para todas las demás plantas, y ver si uno mismo funciona para todas las demás plantas de generación.
Posterior a la junta el encargado de PAP, Pablo, hizo entrega de la guía operativa del pronóstico de corto plazo de generación intermitente versión 20190131. En ella se encuentran las principales metodologías para el pronóstico de generación intermitente (centrales eléctricas tipo fotovoltaicas, eólicas, entre otras) de acuerdo con lo establecido en el Manual de Pronósticos (MP), disposiciones generales, modelos de regresiones como lineales (mínimos cuadrados), resultados de pronósticos por método de promedio lineal múltiple. Entre otros apartados como modelos de promedios móvil simple, promedios móviles ponderados (ambos con sus respectivas tablas de datos) y modelos polinomiales. Además, un glosario para las palabras sujetas a interpretación y palabras rimbombantes. 
En esta semana se tomó el archivo Generación Intermitente de la GCROC 201.xlsx para limpiarlo, debido a que en el mismo archivo se encontraba toda la información de todas las plantas en una sola hoja, lo cual generaba retraso en los procesos de lectura de los programas. Como solución, se creó un programa para poder dividir todas las plantas en un .xlsx diferente con la información necesaria y acomodada de tal manera que facilita la lectura del programa principal que corre el pronóstico de cada planta en forma individual. Además, en esta semana se hizo entrega del formato del Reporte de Proyecto de Aplicación Profesional. 

#### Bloque 7 (Optimización) 

20 de abril de 2020 – 2 de mayo de 2020 

Esta semana adicional a los esfuerzos en el proyecto, se recopiló toda la información que se tenía sobre las acciones que se estuvieron realizando. Se archivaban las anotaciones semanales detalladas de los procesos que se estaban siguiendo, los cuales se pueden ver reflejados en estos ocho bloques. 
Los pronósticos hasta este momento eran muy cercanos a los reales, el problema que resaltaba más era el tardío efecto del pronóstico en empezar a correr, en otras palabras, hacía bien el pronóstico, pero desfasado por una hora aproximadamente. Dicha situación causó recurrir a la posibilidad de generar variables dummies para hacerle entender al código que tenía que empezar antes de tiempo, lo cual sí generó un cambio positivo al pronóstico, a pesar de que después de la primera hora recaía de nuevo en el problema inicial y seguía retrasado por una hora. Para algunas plantas a las 9:00 p.m. todavía generaban electricidad, en cambio otras desde las 6:00 am ya tienen poca generación, por lo que no es algo constante. Uno de los planteamientos que se generó fue tomar como referencia el día anterior y correr el modelo para las 24 horas, si el día anterior, el valor fue 0, entonces que el día siguiente el valor también sea 0, con esto se logra ajustar un poco el modelo, en vez de usar dichas dummies.
Se buscó cuáles serían las dummies ideales para poder generar el efecto deseado. Dentro de la hipótesis de por qué estaba sucediendo esto, la más probable era por el desfase del cambio de horario, ya que a pesar de que la hora fuera la misma, el sol no estaba alineado a la hora, sino a los horarios de verano e invierno. 
En esta semana también se hizo la evaluación del PAP, tanto del profesor, como del proyecto PAP. También se mandó este documento a Writing Desk ITESO y nos ayudó en algunos apartados con la gramática y ortografía. 

#### Bloque 8 (Resultados)

4 de mayo de 2020 – 16 de mayo de 2020

En ese último bloque se corrigió este documento para mejorar la lectura. Además de esto se pulieron todos los archivos puesto que como se menciona anteriormente, cada tipo de planta necesitaba un modelo distinto, esta semana se utilizó para poder tomar cada planta y probar los diferentes modelos ya que con cada modelo la planta arroja un resultado diferente lo que es correcto, por ello se hizo una tabla en una hoja de cálculo .xlsx para poder integrar macros y hacerlo aún más automatizado al momento de arrojar el valor de la planta que más le funciona.
Los valores representados en esta tabla es el numero de la planta, el dato real (que es la información que CENACE nos da en un formato), después el dato de predicción (que es el valor que genera el mejor código para esta planta) y por último se muestra el dato del error (que es el porcentaje siempre positivo del fallo generado por hora). Otros datos interesantes que se pueden analizar del desglose por hora es el error diario, por hora, horas con sol, e intervalos de 3 horas por día. 
Los modelos mostrados es modelo ARIMA puro, modelo ARIMA y promedio (7 días) en horas 7 a 9, modelo ARIMA y promedio (7 días) en hora de 7 a 9 y 16 a 18 y los dos datos finales que son la producción total real y la producción total de la estimación. Por último, se muestran tres gráficas, la primera de la predicción vs la real, la segunda gráfica es el error por horas y por último el error por horas juntando el modelo ARIMA y ambos promedios. 
Esta última semana dentro del último bloque se hace entrega de los archivos a CENACE por medio de una videollamada en la que todos los equipos con sus diferentes temas darán explicación solamente de sus resultados. Las 26 plantas son demasiadas para presentar, por lo tanto, se toma solamente una muestra y se da lujo de detalle de cómo es que se obtuvo ese resultado, cuáles fueron los criterios y la lógica para la obtención de dichos resultados. También se entregan todos aquellos archivos adicionales al código sobre el funcionamiento óptimo para que CENACE pueda replicar estos algoritmos a los ya existentes. 
