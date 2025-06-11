# *Proyecto_PythonforData*

### **Objetivo del Proyecto**
Este proyecto tiene como objetivo limpiar y preparar los datos de campañas de marketing telefónico para su posterior análisis exploratorio y visualización. A través de este análisis, se busca extraer información relevante que permita optimizar estrategias de marketing y mejorar la efectividad en futuras campañas. 

### **Conjunto de Datos**
El análisis se basa en dos conjuntos de datos:

1. **bank-additional.csv**
Este dataset contiene información sobre campañas de marketing telefónico realizadas por una entidad bancaria. Las campañas incluían múltiples llamadas a los mismos clientes para intentar lograr la contratación de un producto bancario.

Columnas Principales:
- age: Edad del cliente.
- job: Profesión del cliente.
- marital: Estado civil del cliente.
- education: Nivel educativo.
- default: Historial de incumplimiento de pagos (1: Sí, 0: No).
- housing: Indica si el cliente tiene una hipoteca (1: Sí, 0: No).
- loan: Indica si el cliente tiene otros préstamos (1: Sí, 0: No).
- contact: Método de contacto (teléfono, móvil, etc.).
- duration: Duración en segundos de la última interacción.
- campaign: Número de contactos durante la campaña.
- pdays: Días desde el último contacto previo.
- previous: Número de contactos anteriores.
- poutcome: Resultado de la campaña anterior.
- emp.var.rate: Tasa de variación del empleo.
- cons.price.idx: Índice de precios al consumidor.
- cons.conf.idx: Índice de confianza del consumidor.
- euribor3m: Tasa de interés Euribor a tres meses.
- nr.employed: Número de empleados.
- y: Resultado de la campaña (Sí/No).
- date: Fecha de la interacción.
- contact_month: Mes de la interacción.
- contact_year: Año de la interacción.
- id_: Identificador único de cada registro.

2. **customer-details.xlsx**
Este archivo contiene información adicional de los clientes, segmentada por año de ingreso al banco (2012, 2013 y 2014).

Columnas Principales:
- Income: Ingreso anual del cliente.
- Kidhome: Número de niños en el hogar.
- Teenhome: Número de adolescentes en el hogar.
- Dt_Customer: Fecha en la que el cliente se unió al banco.
- NumWebVisitsMonth: Número de visitas mensuales al sitio web.
- ID: Identificador único del cliente.

### **Procesamiento de los Datos con Python**

La limpieza y transformación de los datos se llevó a cabo en Python utilizando un Jupyter Notebook. Las siguientes librerías fueron empleadas para el análisis y la visualización:

- pandas: Para la manipulación y análisis de datos estructurados.
- numpy: Para operaciones matemáticas y manejo de matrices.
- sklearn: Para la imputación de valores nulos y técnicas avanzadas de preprocesamiento:
    - KNNImputer
- seaborn: Para la visualización de gráficos estadísticos.
- matplotlib: Para la visualización básica y personalizada de datos.
- plotly: Para visualizaciones interactivas y dinámicas:
    - plotly.express
    - plotly.graph_objects
    - plotly.subplots

### **Análisis Exploratorio**

- ¿Qué tipo de clientes muestran mayor interés o probabilidad de adquirir un producto financiero?

- ¿Cuáles son los elementos clave que determinan la efectividad de una estrategia de marketing?

- ¿Qué características demográficas predominan entre los usuarios habituales del banco?

- ¿De qué manera afectan los distintos medios de contacto a los resultados de conversión?

- ¿Qué patrones de comportamiento se detectan en los clientes con el paso del tiempo?

### **Visualizaciones y Resultados**

Se emplearon diversas herramientas gráficas para visualizar y analizar las respuestas a las preguntas planteadas, entre las que destacan:

- Histogramas: Utilizados para examinar cómo se distribuyen variables como la edad, los ingresos y la duración de las llamadas.

- Gráficos de líneas: Ideales para identificar patrones y tendencias a lo largo del tiempo en la duración de las campañas y en la reacción de los clientes.

- Diagramas de dispersión: Permitieron explorar las relaciones entre distintas características de los clientes, como la duración de las llamadas frente al número de contactos realizados.

- Gráficos circulares: Empleados para comparar las tasas de conversión entre la campaña actual y la anterior, facilitando una visión rápida de los resultados.


### **Conclusiones y Recomendaciones**
Este estudio ofrece información clave que puede ayudar a afinar la segmentación de clientes y a potenciar la eficacia de futuras campañas de marketing, teniendo en cuenta aspectos como las características demográficas y los canales de comunicación que generan mejores resultados.

### **Estructura del Proyecto**

/Proyecto_PythonforData
│
├── Data
│   ├── bank-additional.csv
│   └── customer-details.xlsx
│   └── bank-limpio.csv
│   └── bank-limpio-sin-nulos.csv
│
├── EDA_bank.ipynb
│
├── Informe_Final.pdf
|
└── README.md