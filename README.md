Proyecto de Análisis de Proteómica y fosfoproteómica




#############################################################################################

#    ____()()
#      /      @@
#`~~~~~\_;m__m._>o   


Este repositorio contiene el código y la documentación para realizar análisis de proteómica y fosfoproteómica en R, generar visualizaciones y consultas API a string en Python. El proyecto se centra en el análisis de datos proteómicos y fosfoproteómicos obtenidos de diferentes experimentos, buscando identificar patrones, variaciones y correlaciones que permitan entender mejor los efectos biológicos de distintas condiciones experimentales.
#############################################################################################
Autoría

Este proyecto ha sido realizado por Julia Verheul, estudiante de doctorado del grupo de Neuropsicofarmacología del IBIMA en Málaga.

#############################################################################################

Descripción del Proyecto

El proyecto incluye dos análisis principales:

    Efecto del alcohol: Análisis del impacto del consumo de alcohol en ratas machos, centrado en cambios proteómicos en el hipocampo.
    Efecto del alcohol y Estrés Agudo por Inmovilización: Análisis combinado para estudiar el efecto de la exposición al alcohol junto con el estrés agudo por inmovilización en ratas machos, enfocándose en las alteraciones en el hipocampo.


#############################################################################################

Estructura del Repositorio

    data/: Carpeta que contiene los archivos de datos procesados y/o los resultados intermedios. Los datos en esta carpeta, tanto de proteómica como de fosfoproteómica, ya están normalizados y listos para su análisis.
    scripts/: Contiene los scripts en R para realizar los análisis principales, como el análisis estadístico y la generación de heatmaps.
    python/: Contiene scripts en Python para realizar consultas API, incluyendo interacciones con la base de datos STRING para la obtención de datos adicionales sobre las proteínas de interés.
    results/: Carpeta para almacenar los resultados finales y gráficos generados, incluyendo los resultados específicos de la fosfoproteómica.


#############################################################################################

Requisitos

Este proyecto utiliza R y Python para el análisis de datos, además del software SEAOP. Asegúrate de instalar los siguientes paquetes y software antes de ejecutar los scripts:


Instalación de Paquetes en R

install.packages(c("effsize", "readxl", "data.table", "dplyr", "xlsx", "openxlsx", "igraph", 
                   "ggraph", "ggplot2", "ggrepel", "pheatmap", "RColorBrewer", 
                   "FactoMineR", "factoextra", "edgeR"))

#############################################################################################
Instalación de SEAOP

Para el análisis estadístico y la detección de outliers, este proyecto requiere el uso de SEAOP. Asegúrate de seguir las instrucciones de instalación en su repositorio para configurarlo adecuadamente antes de ejecutar los análisis.
https://academic.oup.com/bib/article/25/3/bbae129/7638267?login=true
https://github.com/whisperH/SEAOP

#############################################################################################
Ejecución

    Preparación de los Datos: Coloca tus datos en la carpeta data/.
    Análisis en R: Utiliza los scripts en la carpeta scripts/ para realizar el análisis principal, como el análisis estadístico, filtrado y generación de heatmaps.
    Consultas API en Python: Ejecuta los scripts en la carpeta python/ para realizar consultas a la base de datos STRING y obtener datos adicionales sobre las proteínas de interés.
    Interpretación de Resultados: Los resultados generados se guardan en la carpeta results/ para su interpretación.
