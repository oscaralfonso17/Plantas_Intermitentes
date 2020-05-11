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

* Semana 1 
    * Tuvimos la presentación con el CENACE en sus oficinas
    * Se explicó que es lo que se hará con el CENACE
* Semana 2
    * Se hicieron los equipos para podernos dividir los proyectos que se dejaron acargo de este PAP 
    * Se consultó con el cordinador de PAP como es que se llevaría acabo el procedimiento de cada proyecto 
    * Fijamos los objetivos 
* Semana 3
    * Entender el código del semestre pasado 
    * Entender que es el modelo ARIMA y como funciona en Python 
    * Optimizar el código para lograr una reducción de tiempo, en MAE y MAPE
* Semana 4
    * Cargar codigo en github
    * Pronóstico 1 año completo
    * MAE < 20%
    * MAPE < 20%
    * Estadística descriptiva de los resultados
    * Pull request
    * Ediciones o mejoras o propuesta de reestructuración completa del código.
    * Econtramos APIs para bajar los datos historicos del clima en Gdl 
        * Desventajas; Hay que estar bajando el excel y son cada 3 horas, no cada hora
    * obtuvimos datos meteorológicos 
* Semana 5 
    * Cambiamos el foco de nuestro proyecto
    * Nuestro nuevo objetivo para el proyecto será tomar el código del equipo anterior y hacerlo correr
    * Harémos el código más eficiente y hacer que funcione para ambas plantas; fotovoltaicas y eólicas
    * El código del equipo tenía algunos errores que identificamos; 
        * Corrian unos días en específico por eso obtenían un buen porcentaje
        * Para ciertas plantas no corría la función
        * Algunas de las APIs que utilizaban son dificiles de instalar 
        * Su función 'mape_prom' no corría, tenía errores en el código
        * Reciclaban algunos datos
    * Para hacerlo correr necesitamos la integración de algunas APIs 
    * Despues de hacer correr las APIs dentro del código 
    * Resolvimos dudas con respecto algunos APIs
    
* Semana 6 
    * Se hizo correr las APIs faltantes
    * Se pudo correr el 'mape_prom' 
    * Junta con el CENACE para hacer la presentación de los proyectos 
    * Se explica; Objetivo general del proyecto, objetivos específicos, metodología del trabajo, avances para la fecha
    * Primera entrega de nuestra presentación formal para explicar que es lo que estamos haciendo y que haremos para alcanzar nuestros objetivos. 