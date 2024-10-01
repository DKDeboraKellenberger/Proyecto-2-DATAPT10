 ![alt text](<Images/Logo Henry.png>)

# Proyecto-2-DATAPT10

## Telecomunicaciones

# Descripción

El análisis está enfocado a proporcionar información detallada del comportamiento del sector de las telecomunicaciones a nivel nacional en cuanto al servicio de internet.

El objetivo de este proyecto es poner en carpeta los comportamientos de los usuarios en el territorio argentino en la última década.

Con una correcta interpretación de los datos se intentará primeramengte contextualizar el comportamiento de la industria. Una vez entendido el entorno, tomar las decisiones adecuadas para la empresa, reflejandose las mismas en  objetivos claros y la mejora en la calidad del servicio. 
No debemos dejar de mencionar que en la linea de tiempo a analizar, hubo un eje mundial que cambio los paradigamas de consumo y de vida. La pandemia del Covid-19 marcó un antes y un despues en las telecomunicaciones, en especial al Internet. Ésta tecnología se volvió un servicio esencial, medio cuasi indispensable para todos. 
En los datos, esto se lee como un aumento del consumo a partir del 2019 (recordemos que los primeros casos en Wuhan, China, fueron en diciembre de 2019).

La idea es realizar un analisis descriptivo para, con esas conclusiones, poder predecir dónde es conveniente hacer foco de aquí a futuro en cuanto a expansión, inversión o desarrollo de nuestro servicio de intenet según digan los datos, basados en la mirada del 'nuevo mundo' post pandemico mucho mas informatizado y conectado.

# Proceso

Los datos crudos (fuente: ENACOM), proporcionados en una base de datos en formato Excel, fueron procesados debidamente para lograr dos Datasets: 'internet_prov', el cual contiene informacion por año y trimestre acerca de las conexiones a internet a nivel pais discriminando por provincias. Esa información esta compuesta por Media de bajada medido en Mbps, tecnologías de conexión y la penetracion de la tecnología a analizar en cuanto a 100 habitantes y hogares. El Otro dataset, 'ingresos' contiene lo refereido medido en miles de pesos. Estos dos archivos se hicieron por separado para una optimizacion de las tablas, ya que no poseen la misma cantidad de datos. Una vez transformados, fueron convertidos a formato parquet.



# Estructura del Proyecto

# Fuente de datos
Datasets principales, que recoge datos del ENACOM
# Autor
Débora L. Ferrucci Kellenberger






