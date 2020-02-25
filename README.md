# PAP ITESO 2020
## PROGRAMA DE MODELACION MATEMATICA PARA EL DESARROLLO DE PLANES Y PROYECTOS DE NEGOCIO I
### CENACE: Pronósticos de generación de plantas intermitentes
### Flores Orozco, Oscar Alfonso; Ramírez Cambero, Job; González Juárez, Edgar Ranulfo

***

### OBJETIVO GENERAL: 

* Generar un modelo para el pronóstico de variables horarias.

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

* Para poder trabajar de forma remota


***

### AVANCES 

* Semana 1 
    * Se definieron los equipos de trabajo, y los objetivos generales del PAP.

* Semana 2
    * Tuvimos una junta con el CENACE en sus oficinas, donde se nos presentaron sus metodologías de trabajo y sus objetivos que tienen con el convenio PAP.

* Semana 3
    * Tuvimos una segunda junta, ahora con el equipo de desarrollo de aplicaciones del CENACE, quienes nos explicaron los lineamientos de los entregables que buscan por parte de nosotros

* Semana 4
    * Se empezó con la búsqueda de APIs para la descarga de datos históricos del clima.
        * Nos topamos con el problema del costo de las mismas API, pero se encontró este sitio: https://rp5.ru/ que te da históricos de la mayoría de las ciudades.
        * Se comenzó a limpiar la base de datos obtenida y a observar que columnas de información serán útiles para los siguentes pasos del proyecto.
    
* Semana 5 
    * Cambiamos el foco de nuestro proyecto.
    * Nuestro nuevo objetivo para el proyecto será tomar el código del equipo anterior, entenderlo y buscar mejorarlo.
    * Harémos el código más eficiente y hacer que funcione para ambas plantas; fotovoltaicas y eólicas, buscando reducir también el tiempo de ejecución.
    * El código del equipo tenía algunos errores que identificamos; 
        * Corrian unos días en específico por eso obtenían un buen porcentaje
        * Para ciertas plantas no corría la función
        * Algunas de las APIs que utilizaban son dificiles de instalar 
        * Su función 'mape_prom' no corría, tenía errores en el código
        * Reciclaban algunos datos
    * Para hacerlo correr necesitamos la integración de algunas librerías de python.
    * Se logró la instalación de las librerías dentro del código 
    * Resolvimos dudas con respecto algunos librerías
    
* Semana 6 
    * Se hizo correr las librerías faltantes
    * Se pudo correr el 'mape_prom' 
    * Junta con el CENACE para hacer la presentación de los proyectos y objetivos por equipos:
        * Se explica:
          * Objetivo general del proyecto
          * objetivos específicos
          * metodología del trabajo
          * avances para la fecha
    
    
