# Individual2_Henry - Data Science

# Analisis de Datos de Telecomunicaciones de Argentina. 

Este repositorio contiene un Analisis Exploratorio de Datos (EDA) para la información registrada acerca de las conexiones a internet entre el primer trimestre de 2014 y el segundo trimestre de 2024.

# Tabla de Contenido: 

1. [Contexto](#contexto)
2. [Procesos Implementados](#2-procesos-implemetados)
3. [Análisis Exploratorio](#analisis-exploratorio)
4. [Dashboards](#4-dashboards)
5. [KPI](#5-kpi)

# 1. **Contexto**

Las telecomunicaciones incluyen la transmisión de información a través de medios como telefonía, televisión, radio e internet. Este último, una red global de computadoras interconectadas, ha transformado nuestras formas de comunicación, trabajo, educación y entretenimiento.

La industria de las telecomunicaciones es esencial para la sociedad, facilitando la información a nivel global, especialmente en tiempos de crisis. En Argentina, el sector avanza rápidamente, con 62,12 millones de conexiones en 2020, destacándose por encima del promedio mundial en el desarrollo de infraestructuras de telecomunicaciones.

### Información evaluada:

Los datos evaluados a continuación provienen de la data "Internet", que contiene información detallada sobre la penetración y accesos a internet en Argentina. Los conjuntos de datos incluidos son:

 - Datos detallados de accesos a internet por velocidad y localidad.
 - Estadísticas de acceso por velocidad y provincia.
 - Porcentaje de accesos por rangos de velocidad en cada provincia.
 - Totales de velocidad media descargada por región.
 - Accesos a internet por tecnología en distintas localidades.
 - Totales de accesos desglosados por tecnología.
 - Accesos por tecnología en diferentes provincias.
 - Datos de accesos dial-up y Banda Ancha Fija.
 - Totales de accesos dial-up y Banda Ancha Fija.
 - Datos de penetración de internet en la población.
 - Penetración de internet en hogares.
 - Totales de penetración de internet.
 - Totales de accesos a internet por velocidad.
 - Accesos por velocidad en cada provincia.
 - Datos de ingresos generados por los servicios de internet.

# 2. **Procesos Implemetados**

Para empezar, se descargó la base de datos de internet disponible (la cual contenía la información previamente referenciada). Una vez descargada la base y montada en Python se procedió a hace una visualización de los datos para entrar en contexto sobre la información encontrada. 

Mas adelante se detalla el proceso de analisis y exploración de datos, por lo pronto, solo cabe mencionar que se seleccionaron algunas de las hojas de la dataset, no todas. Solo las qe se consideraron relevantes. 

Una vez teniendo un EDA preliminar en Python, se procedió a elaborar graficas complementarias en Power BI. Cabe mencionar que a pesar de utilizar la misma inforamción tanto en Python como en Power BI, las graficas no son las mismas. El diseño en Power BI es más interactivo y se trató de explorar la información de manera que arrojara mejores resultados y permitiera un analisis más detallado, sin embargo no se cumplió esta expectativa fuera de una visualización más dinamica que en VSC. 

# 3. **Analisis Exploratorio**

Dado que no todas las columnas tenian información relevante para hacer un analisis detallado se seleccionaron solo algunas. Las seleccionadas fueron las siguiente: 

 1. Velocidad_sin_Rangos: Esta hoja parece contener información detallada sobre las velocidades de conexión a internet. Entender la distribución y variabilidad de las velocidades es crucial para el análisis, ya que la velocidad de conexión impacta directamente en la calidad del servicio.
 2. Totales Accesos Por Tecnología: Para entender el panorama general de los tipos de tecnología que predominan en el acceso a internet.
 3. Acc_vel_loc_sinrangos: Proporciona datos sobre el acceso por localidad, lo que te permitirá explorar cómo varía el acceso a internet en diferentes regiones.
 4. Velocidad % por prov: Esta hoja ofrece un desglose porcentual de las velocidades por provincia, lo que es útil para identificar desigualdades regionales en el acceso a internet.
 5. Totales VMD: Los totales de velocidad media descargada (VMD) son un indicador clave del rendimiento de la red.
 6. Penetración-poblacion y Penetracion-hogares: Estas hojas ofrecen una visión de la penetración del internet en la población y en los hogares, fundamentales para entender la accesibilidad y adopción del servicio.
 7. Ingresos: Esta hoja proporciona los datos principales sobre los ingresos generados por los servicios de internet.

Para cada una de las anteriores columnas se hizo más o menos lo mismo: se procedió a visualizar las columnas y el tamaño de la información, se buscaron y eliminaron valores nulos, se evaluó si habian outliers y en algunos casos se eliminaron para que no se deformaran las tendencias. A pesar de que la información de base venia practicamente limpia, fue necesario hacer algunos ajustes minimos de limpieza para poder presentar gráficas sin errores. 

Finalmente, una vez la información estaba lista y clara se procedió a elaborar graficas que permitieran visualizar el comportamiento de las diferentes variables. 

Se creó una o dos graficas con su respectivo analisis para cada una de las hojas seleccionadas de la database de Internet. El desarrollo de todas estas graficas, su explicación y conclusiones se encuentran en la sección EDA del Proyecto (Archivo: "EDA_internet"). 

# 4. **Dashboards**

Para una mejor visualización de datos, se hicieron graficas con la misma base de información en Power Bi. 

La intención de realizar estas gráficas era poder tener una visualización más detallada de los datos con los que se contaba, lastimosamente la información de base es muy simple y las transformaciónes que se intentaron realizar en Power Bi no arrojaron resultados que hicieran aportes significativos que no hayan sido previamente explorados al momento de realizar el EDA del proyecto. Se trató de consolidar las bases de datos en una sola para poder tener una mejor visualización, pero esto no fue posible. 

Sin embargo, las graficas presentadas, al ser interactivas permiten tener un mejor acceso a los datos de manera automatica. 

Todas estas gráficas mencionadas se encuentran en la sección Dashboard del Proyecto (archivo: "Dashboard_Internet")

# 5. **KPI**

Una de las tareas de este proyecto era armar un KPI que indicara cual es el valor de incremento de los accesos de los hogares si para el tercer trimestre de 2024 habia un incremente del 2% con respecto al trimestre anterior. Este KPI fue debidamente tabulado y graficado en la ultima página del mismo archivo del Dashboard donde se encuentran las graficas mencionadas. 

Asi mismo se intentó crear otros KPI con la misma base de datos, sin embargo, fue complicado porque la información suministrada para accesos de hogares no arroja mucha información. Por ejemplo, para medir el porcentaje de penetración en valores relativos con respecto al total de la población, se requiere conocer la cantidad total de hogares existentes. Hacer un estimado de esto no tenia sentido para crear un KPI. Por ejemplo. 

# 6. **Conclusiones Generales del Proyecto**

Este proyecto demuestra que en Argentina, en la ultima década hubo un incremente considerable tanto de los accesos a internet, como de la velocidad de carga y descarga así como de los ingresos que el sector genera. 
Se muestra que con el paso de los años, se inicia con unos porcentajes de participacion en velocidad, ingresos y conexiones relativamente bajos pero que crecen de forma sostenida cada año. 

Con respecto a la velocidad, se muestra que hubo un periodo en el que la velocidad de descarga alcanzó los 10000 pero se estableció como limite el 1024 y se mantuvo durante los años siguientes. 

Se observa que al inicio de la decada habia unas tecnologias, que aunque se han seguido usando en algunos hogares, cuando aparecen las nuevas tecnologías arrazan con las anteriores y se posicionan como las más representativas. Pero hay hogares que prefieren continuar el uso de tecnologias anteriores. No hay información para tener claro si hay una relación directa entre el tipo de tecnologia (nueva o antigua) y la velocidad. NO pude llegar a este tipo de conclusión. 

En toda las tablas el criterio de coincidencia es el año. Si bien esto permite hacer evaluaciones de series de tiempo, no es muy productivo porque vale la pena rescatar la provincia para cada ejercicio pero este criterio solo existe en algunas de las bases de datos y no en toda. 

Cada conclusión de cada grafica se encuentra con más detalle en el EDA. 