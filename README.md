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
### Páginas del Dashboard
 #### 1. Análisis Regional
- **Descripción**: Esta página contiene gráficos de barras que muestran:
  - Tecnologías de conexión por cada provincia.
  - Velocidad de bajada por cada provincia.
  - Cantidad de conexiones por provincia.

 #### 2. Mapa de Conexiones
- **Descripción**: Esta página presenta un mapa donde el tamaño de cada burbuja indica la cantidad de conexiones totales por provincia.
- **Tooltip**: Al posar el cursor sobre una burbuja, se muestra un tooltip con detalles de la provincia, incluyendo el número exacto de conexiones y la proporción de los tipos de tecnologías de conexión.

 #### 3. Ingresos
- **Descripción**: Esta página incluye un gráfico de líneas que muestra los ingresos en miles de pesos durante la última década, desglosado por año.
- **Filtro**: Se puede aplicar un filtro por provincia.
- **KPI**: Incluye un KPI que mide un objetivo de incremento del 12% interanual en los ingresos.

 #### 4. Tendencias
- **Descripción**: Esta página contiene dos gráficos de líneas:
  - **Tendencias de Velocidades de Conexión**: Muestra las tendencias de las diferentes opciones de velocidades de conexión durante la última década.
  - **Tendencias de Tecnologías de Conexión**: Muestra las tendencias de las tecnologías de conexión durante la última década.

 #### 5. Objetivo de Conexiones
- **Descripción**: Esta página incluye un KPI que mide un objetivo de aumento del 2% en las conexiones por cada 100 hogares en relación al trimestre anterior.
- **Gráfico de Líneas**: Visualiza el objetivo de conexiones.
- **Filtro**: Se puede aplicar un filtro por provincia.

 #### 6. Objetivo de Incremento
- **Descripción**: Esta página permite aplicar un filtro por provincia y contiene:
  - **KPI**: Indica si la provincia tiene más de 5 millones de conexiones o no, y muestra el número exacto de conexiones.
  - **Gráfico de Líneas**: Visualiza el objetivo de incremento de conexiones.

### Uso del Dashboard

1. **Navegación**: Utiliza los botones de navegación de la parte inferior del dashboard para navegar entre las diferentes páginas.
2. **Filtros**: Aplica los filtros disponibles para personalizar la visualización de los datos según las necesidades.
3. **Interacción**: Interactúa con los gráficos y mapas para obtener información detallada y específica de cada provincia.

## Contacto
debkelen1@gmail.com

# Glosario
 **Breve explicación de algunos términos, para una mejor comprensión del análisis:**

### Tecnologías de Conexión
##### ADSL (Asymmetric Digital Subscriber Line): 
ADSL es una tecnología de conexión a internet que utiliza las líneas telefónicas de cobre existentes para transmitir datos. Es asimétrica porque ofrece velocidades de descarga más rápidas que las de subida. Es común en áreas donde la infraestructura de fibra óptica no está disponible.
#### Cablemodem: 
El cablemodem es una tecnología que utiliza las redes de televisión por cable para proporcionar acceso a internet. Ofrece velocidades de conexión más rápidas que ADSL y es ampliamente utilizada en áreas urbanas y suburbanas.
#### Fibra Óptica: 
La fibra óptica utiliza cables de vidrio o plástico para transmitir datos a velocidades extremadamente altas mediante pulsos de luz. Es la tecnología de conexión más rápida y confiable disponible actualmente, ideal para aplicaciones que requieren gran ancho de banda, como streaming de video en alta definición y juegos en línea.
#### Wireless: 
La tecnología inalámbrica (Wireless) permite la conexión a internet sin necesidad de cables físicos, utilizando ondas de radio. Incluye tecnologías como Wi-Fi, LTE y 5G. Es muy conveniente para dispositivos móviles y en áreas donde la instalación de cables es difícil o costosa.

### Descripción de Mbps y Velocidades de Conexión
#### Mbps (Megabits por Segundo): 
Mbps es una unidad de medida que indica la velocidad de transferencia de datos. Un megabit equivale a un millón de bits. Las velocidades de conexión a internet se miden en Mbps, y una mayor cantidad de Mbps significa una conexión más rápida.
#### Explicación de las Velocidades:
**Baja Velocidad (menos de 10 Mbps):** Adecuada para navegación básica, correo electrónico y redes sociales.
**Velocidad Media (10-50 Mbps):** Suficiente para streaming de video en alta definición, videollamadas y juegos en línea.

*Alta Velocidad (50-100 Mbps): Ideal para hogares con múltiples dispositivos conectados, streaming en 4K y descargas rápidas.
Muy Alta Velocidad (más de 100 Mbps): Recomendable para aplicaciones que requieren gran ancho de banda, como streaming en 4K, juegos en línea sin latencia y trabajo remoto con grandes transferencias de archivos. (no entran en este análisis, pero es bueno explicarlo para un mejor conexto general)*

# Fuente de datos
Datasets principales, que recoge datos del ENACOM
# Autor
Débora L. Ferrucci Kellenberger






