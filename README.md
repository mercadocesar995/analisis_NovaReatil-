# analisis_NovaReatil-

## Factores de comportamiento — NovaRetail+
Objetivo del proyecto

Este proyecto analiza el comportamiento de 15.000 clientes de NovaRetail+ utilizando información relacionada con sus características, interacción con la plataforma, compras, satisfacción, membresía Premium y abandono.

El objetivo principal es responder a la siguiente pregunta

¿Qué factores del comportamiento del cliente están más fuertemente asociados con el ingreso anual generado?

El análisis busca identificar las variables que presentan mayor asociación con el ingreso_anual, explorar posibles patrones entre las características de los clientes y generar hallazgos que puedan apoyar las estrategias de crecimiento y retención.
El proyecto corresponde a un análisis correlacional y exploratorio.

## Dataset utilizado

### El proyecto utiliza un conjunto de datos con 15.000 registros y 12 variables.

**Identificación y características del cliente**

**id_cliente**: identificador único del cliente.

**edad**: edad del cliente.

**nivel_ingreso**: ingreso anual estimado del cliente.




**Comportamiento en la plataforma**

**visitas_mes**: número de visitas realizadas a la aplicación o sitio web durante el mes.

**compras_mes**: número de compras realizadas durante el mes.

**gasto_publicidad_dirigida**: gasto en publicidad dirigida asignado al cliente.




**Experiencia y relación con la plataforma**

**satisfaccion**: calificación de satisfacción del cliente en una escala de 0 a 5.

**miembro_premium**: indica si el cliente pertenece al programa Premium (1 = sí, 0 = no).

**abandono** indica si el cliente abandonó la plataforma (1 = sí, 0 = no).




**Variables categóricas**

**tipo_dispositivo**: dispositivo utilizado por el cliente: móvil, escritorio o tablet.

**region**: región geográfica del cliente: norte, sur, este u oeste.




**Variable objetivo**

**ingreso_anual**: ingreso anual generado por cada cliente para la empresa.



## Herramientas utilizadas

-Python
-Pandas
-NumPy
-Matplotlib
-Seaborn
-SciPy
-Google Colab
-GitHub

## Etapas del análisis

El proyecto se desarrolló en las siguientes etapas:

**1. Exploración inicial**

Dimensiones del conjunto de datos.

Estructura de las variables.

Tipos de datos.

Valores faltantes.

Rangos y estadísticas descriptivas.

Distribución de variables numéricas, binarias y categóricas.

El dataset contiene 15.000 clientes y 12 variables, sin valores nulos.


**2. Limpieza y transformación**

Conversión de edad de float64 a int64.

Conversión de miembro_premium a variable booleana.

Conversión de abandono a variable booleana.

Validación de las variables categóricas tipo_dispositivo y region.

Revisión de la consistencia de las variables numéricas.


**3. Análisis exploratorio**

Edad: edad de cada cliente, expresada en años.

Nivel de ingreso: nivel de ingresos del cliente utilizado para clasificar su capacidad económica.

Visitas mensuales: cantidad de veces que el cliente interactúa con la plataforma durante un mes.

Compras mensuales: cantidad de compras realizadas por el cliente durante un mes.

Gasto en publicidad dirigida: inversión destinada a mostrar campañas publicitarias personalizadas a cada cliente.

Satisfacción: valoración del nivel de satisfacción reportado por el cliente.

Ingreso anual: ingreso anual estimado o registrado para cada cliente.


**4. Análisis de variables categóricas y binarias**

Se exploraron las variables relacionadas con:

Membresía Premium: indica si el cliente pertenece o no al programa de membresía Premium.

Abandono: indica si el cliente abandonó o continúa utilizando el servicio.

Tipo de dispositivo: dispositivo utilizado por el cliente para acceder a la plataforma, como móvil o escritorio.

Región geográfica: región a la que pertenece cada cliente.


**5. Análisis de correlaciones**

Se utilizaron diferentes métodos estadísticos para analizar la relación entre las variables, según el tipo de datos:

Pearson: Para medir la relación lineal entre dos variables numéricas.

Spearman: Para medir si dos variables presentan una relación consistente, aunque no necesariamente lineal.

Punto-biserial: Analizar la relación entre una variable numérica y una variable con dos categorías.

V de Cramér: Medir el nivel de asociación entre dos variables categóricas.


**6. Principales hallazgos**

Membresía Premium y abandono: los clientes Premium presentan una menor proporción de abandono que los clientes No Premium, aunque la asociación entre ambas variables es débil.

Compras e ingreso anual: se identificó una correlación muy alta (r = 0,97), por lo que es necesario validar la construcción de ambas variables antes de interpretar esta relación.

Publicidad y visitas: existe una relación positiva moderada (r = 0,58), pero la correlación no permite determinar si una mayor inversión publicitaria genera más visitas.

Satisfacción: presenta una relación lineal prácticamente inexistente con el ingreso anual y las compras, por lo que se recomienda explorar otros patrones o segmentaciones.

**7. Conclusiones** 

El análisis permitió identificar diferentes patrones en el comportamiento de los clientes de NovaRetail+, así como relaciones que requieren una investigación adicional. Los resultados pueden servir como punto de partida para segmentar clientes, revisar la estrategia de fidelización y evaluar el impacto de las campañas publicitarias.


## Cómo ejecutar el proyecto


Google Colab: https://colab.research.google.com/drive/1P3fKOE2kA3Z7m-c_fwBwXZx4JoGvXWk5?usp=sharing

Ingresa a Google Colab.

Selecciona Archivo → Abrir notebook → Subir.

Carga el archivo .ipynb.

Ejecuta las celdas en orden desde el inicio hasta el final.
