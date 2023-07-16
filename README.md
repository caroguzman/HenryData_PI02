<em> #PROYECTO INDIVIDUAL Nº2</em>

# <h1 align=center>**`Data Analyst`**</h1>

## Objetivo
Una empresa prestadora de servicios de telecomunicaciones solicita la realización de un análisis completo que permita reconocer el comportamiento de este sector a nivel nacional, con el fin de orientar a la empresa en brindar una buena calidad de sus servicios, identificar oportunidades de crecimiento y poder plantear soluciones personalizadas a sus posibles clientes.

## Desarrollo
Para llevar a cabo el proyecto se definieron diferentes etapas de desarrollo:
- **`EDA - Análisis exploratorio de los datos`**: _(Exploratory Data Analysis-EDA)_ (https://)
  Se extraen los datos desde la API de ENACOM y se los procesa para su posterior análisis. Se investiga las relaciones que hay entre las variables de los datasets. 

- **`Análisis`**:
  1. Buscar localidades en donde hay mucha penetración de internet pero de baja velocidad, o sea el porcentaje de accesos sobre la población es alto, pero el porcentaje de accesos >=100Mbps es bajo. En esas localidades se puede proponer una inversión de bajo costo en el update de los equipos de acceso para brindar mayor velocidad.
  2. Buscar localidades con población alta pero baja penetración de internet. En esas localidades se puede proponer invertir en la instalación de equipos de acceso.
  3. Un plus podría ser verificar si hay localidades cercanas con mayor penetración para que el costo de la conexión del equipo de acceso no sea tan alto

- **`Dashboard`** _(FastAPI)_ (https://)
  Se un dashboard con los datos elegidos para el análisis realizado.
    
- **`KPIs`**
  Se presentan 3 KPIs a la empresa como conclusión del análisis realizado:
  - Recomendación de inversión en internet y no en otros medios de comunicación como la telefonía móvil
  - Recomendación de inversión en equipos de acceso a internet de alta velocidad (>= 100Mbps)


## Fuentes
[ENACOM](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/)

## Conclusiones

