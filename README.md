 ![alt text](<Images/Logo Henry.png>)

# Proyecto-2-DATAPT10

## Telecomunicaciones

# Descripción general.

El análisis está enfocado a proporcionar información detallada del comportamiento del sector de las telecomunicaciones, a nivel nacional en cuanto al servicio de internet.

El objetivo es presentar las conclusiones de mi trabajo a una empresa de telecomunicacioneses poniendo en carpeta los comportamientos de los usuarios en el territorio argentino en la última década, en su nivel de consumo actual y en la linea de tiempo de diferentes tecnologías de conexion y velocidades, demostrando esto tendencias y posibles baches (nichos) a tener en cuenta para futuras inversiones en cuanto a intraestructura. Tambien se analizan variables dirigidas a dar un pantallazo de los ingresos economicos, con objetivos planteados a un futuro.

El proceso comenzó con la descarga de los datos proporcionados provenientes de la pagina web del ENACOM (https://indicadores.enacom.gob.ar/datos-abiertos), su posterior transformación y carga correspondiente (ETL).
Se realizó un Análisis Exploratorio de los Datos (EDA) para nutrirme de los mísmos, con gráficos acordes para una interpretación profunda.

---------------------
Con una correcta interpretación de los datos se intentará primeramengte contextualizar el comportamiento de la industria. Una vez entendido el entorno, tomar las decisiones adecuadas para la empresa, reflejandose las mismas en  objetivos claros y la mejora en la calidad del servicio. 
No debemos dejar de mencionar que en la linea de tiempo a analizar, hubo un eje mundial que cambio los paradigamas de consumo y de vida. La pandemia del Covid-19 marcó un antes y un despues en las telecomunicaciones, en especial al Internet. Ésta tecnología se volvió un servicio esencial, medio cuasi indispensable para todos. 
En los datos, esto se lee como un aumento del consumo a partir del 2019 (recordemos que los primeros casos en Wuhan, China, fueron en diciembre de 2019).

La idea es realizar un analisis descriptivo para, con esas conclusiones, poder predecir dónde es conveniente hacer foco de aquí a futuro en cuanto a expansión, inversión o desarrollo de nuestro servicio de intenet según digan los datos, basados en la mirada del 'nuevo mundo' post pandemico mucho mas informatizado y conectado.

# Estructura del Proyecto
## ETL
Los datos fueron proporcionados en un dataset en formato Excel (fuente: ENACOM) con sheets que contenían la información discriminada por diferentes sub-temáticas. Aquí, luego de un análisis de las mísmas, decidí ignorar algunas que no aportaban información relevante para el análisis, y conglomerar las variables de importancia en un archivo con las variables significativas para su medición en cuanto a las diferentes tecnologías, velocidades y la penetración de la industria en los hogares y personas (medido por las conexiones) y clasificado por provincias en años y trimestres; y en otro lo referente a los ingresos, tambien por años y trimestres. 

### Contenido de los Datasets:

- **internet_prov:** 'Año', 'Trimestre', 'Provincia', 'ADSL', 'Cablemodem', 'Fibra óptica','Wireless', 'Otras tecnologías', 'Total por tecnologia', 'HASTA 512 kbps', '+ 512 Kbps - 1 Mbps', '+ 1 Mbps - 6 Mbps', '+ 6 Mbps - 10 Mbps', '+ 10 Mbps - 20 Mbps', '+ 20 Mbps - 30 Mbps', '+ 30 Mbps', 'Otras velocidades', 'Total por velocidades','Mbps (Media de bajada)', 'Accesos por cada 100 hab',
'Accesos por cada 100 hogares'

- **ingresos:** ['Año', 'Trimestre', 'Ingresos (miles de pesos)', 'Periodo'] 

## EDA
 En este paso, se analizaron los dos dataset generados: una inspección inicial de la calidad d elos datos. el número de filas, columnas, se verificó la existencia de valores faltantes, duplicados. Hubo reconocimiento de la variables: cuantitativas(numéricas) y cualitativas(categóricas). De las primeras se obtuvo un informe de estadístivas descriptivas, separadas por temática para un análisis posterior mas claro y enfocado. 
Se realizó un analisis univariante de la variable categórica y de las numéricas, para luego comenzar a relacionar unas con otras (análisis bivariante), y un análisis multivariante con el objetivo de hallar patrones, relaciones y asociaciones entre las características. Cada grafico, consulta o evaluación realizada en el notebook, tiene su correspondiente análisis.

## DASHBOARD - Power Bi






# Glosario
Breve explicación de algunos términos, para una mejor comprensión del análisis:



# Fuente de datos
Datasets principales, que recoge datos del ENACOM
# Autor
Débora L. Ferrucci Kellenberger






