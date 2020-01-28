# Market-Attractiveness-Index
R script to process the index for attractive destinations for Argentinian exports


## Identificar mercados atractivos de exportación con Market Attractiveness Index

Este reporte tiene como objetivo detallar la metodología Market Attractiveness Index (MAI) desarrollada por el International Trade Center (ITC) y replicada en R.

### Introducción
La metodología tiene como objetivo obtener de ranking de países de destino atractivos para la exportación de un producto específico desde un país de origen (en este caso particular, el país de origen es Argentina). Se utilizan 8 indicadores separados en 2 grupos: demanda y acceso. Los primeros 5 se ponderan resultando en un índice de **Demanda**, mientras que los últimos 3 se ponderan para obtener un índice de **Acceso**.

El punto de partida para la construcción del índice es un producto. Todos los productos a nivel internacional se encuentran clasificados en un nomenclador y poseen una _posición arancelaria_ (código numérico) que los identifica en el _Sistema Armonizado_. Esta _posición arancelaria_ (PA) a 6 dígitos, llamada _HS 6_, es la que se utiliza para esta metodología.

El ejemplo que se utiliza en este reporte toma la _posición arancelaria_ del vino fraccionado: **2204.21**.

El estudio evalúa la demanda interancional de este producto y el grado de acceso a cada mercado respecto de los competidores. Para ello, utiliza determinadas variables a partir de las cuales infiere el nivel de **demanda** y de **acceso**.

### Indice de Mercado Atractivo (MAI)
Este índice está compuesto por 2 sub-índices: el **Indice de Demanda de Mercado** (IDM), que muestra la potencialidad de demande de un determindao producto en cada mercado de destino; y el **Indice de Acceso al Mercado** (IAM), que expresa la ventaja relativa que goza un producto del país de origen analizado (en este caso Argentina) en cada mercado de destino en función a la facilidad de acceder al mismo.
