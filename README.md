<em> #PROYECTO INDIVIDUAL Nº2</em>

# <h1 align=center>**`Data Analyst`**</h1>

## Objetivo
Una empresa prestadora de servicios de telecomunicaciones solicita la realización de un análisis completo que permita reconocer el comportamiento de este sector a nivel nacional, con el fin de orientar a la empresa en brindar una buena calidad de sus servicios, identificar oportunidades de crecimiento y poder plantear soluciones personalizadas a sus posibles clientes.

## Desarrollo
Para llevar a cabo el proyecto se definieron diferentes etapas de desarrollo:
- **`EDA - Análisis exploratorio de los datos`**: _(Exploratory Data Analysis-EDA)_ (PI02EDA.ipynb)
  Se extraen los datos desde la API de ENACOM y se los procesa para su posterior análisis. Se investiga las relaciones que hay entre las variables de los datasets. 

- **`MySQL - Conexión a un servidor de base de datos`**: se realiza la conexión y creación de una base de datos y las tablas correspondientes ingestadas con datos depurados en el EDA para automatizar la actualización de los datos en el reporte visual.
- **`Análisis`**:
  1. Buscar localidades en donde hay mucha penetración de internet pero de baja velocidad, o sea el porcentaje de accesos sobre la población es alto, pero el porcentaje de accesos >=100Mbps es bajo. En esas localidades se puede proponer una inversión de bajo costo en el update de los equipos de acceso para brindar mayor velocidad.
  2. Buscar localidades con población alta pero baja penetración de internet. En esas localidades se puede proponer invertir en la instalación de equipos de acceso. ESta inversión será más costosa ya que además de la instalación del equipo se deberá considerar el cableado tanto desde el nodo más próximo como hacia el domicilio del cliente (conocido como última milla).
  3. Un plus puede ser verificar si hay localidades cercanas con mayor penetración para que el costo de la conexión del equipo de acceso no sea tan alto

- **`Dashboard`** _(FastAPI)_ (PI02/Dashboard/Dashboard_Telecomunicaciones.pbix)
  Se realiza un data visualization con los datos elegidos para el análisis realizado.
    
- **`KPIs`**
  Se presentan 2 KPIs a la empresa:
  - Pentración de accesos a internet por provincias
  
  - Penetración de accesos a internet de alta velocidad > 100Mpbs


## Conclusiones
Basado en el análisis de los KPIs mensionados se pueden obtener las siguientes conclusiones / recomendaciones:

  - Recomendación de inversión en nuevos accesos de conexión a internet donde la penetración es baja y hay mucha población. 
    Aquí podemos ver el caso de la provincia de Mendoza, en donde la relación entre la cantidad de accesos y la población es de las más bajas (23.5%). Una posible explicación de este fenómeno es el relieve montañoso de la provincia, lo que dificulta la conexión vía ondas. Por lo que se propone la conexión cableada que si bien resulta más costosa evita los problemas de interferencia y a su vez brinda conexiones de alta velocidad.
  - Recomendación de inversión menor en equipos de acceso a internet de alta velocidad (>= 100Mbps) donde ya hay equipos instalados. Hacer un     upgrade de los accesos ya presentes que no son de alta velocidad. 
    Mediante el análisis de este KPI se puede ver que la localidad de Las Heras presenta una excelente oportunidad de inversión, debido a que la relación entre las conexiones de alta velocidad y la población es muy baja. Otro dato que refuerza este hallazgo es que se cuenta con la disponibilidad de tecnologías ya instaladas. 
    En resumen se recomienda aprovechar esta necesidad insatisfecha para poder brindar el servicio de conexión a internet de alta velocidad.

## Fuentes
[ENACOM](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/)
