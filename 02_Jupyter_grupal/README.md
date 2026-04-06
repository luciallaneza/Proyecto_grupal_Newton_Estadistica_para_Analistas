# 📊  🌏 Proyecto de Análisis: REST Countries API

Este proyecto automatiza la extracción, limpieza y estructuración de datos globales utilizando la API pública REST Countries. El objetivo es transformar datos crudos en formato JSON en un dataset analizable para obtener insights geográficos y demográficos.

🚀 Origen de los Datos
Se ha utilizado la API REST Countries, un servicio gratuito que proporciona información detallada sobre los países del mundo.
Endpoint Consumido
Para optimizar la carga, se ha configurado el siguiente endpoint con filtros específicos:
https://restcountries.com

Variables Extraídas:
Name: Nombre oficial del país.
Capital: Capital o capitales administrativas.
Currencies: Monedas de curso legal.
Languages: Idiomas oficiales.
Region: Continente o región geográfica.
Population: Población total.
Area: Superficie total en km².
Gini: Índice de desigualdad económica.

# 🛠️ Procesamiento y Transformación
El flujo de trabajo convierte una respuesta jerárquica (JSON) en una estructura tabular lista para el análisis estadístico.

1. Extracción (ETL)
La petición se realiza mediante el método GET utilizando la librería requests de Python. Se incluye una validación de estado (raise_for_status()) para garantizar la integridad de la conexión antes de procesar los datos.

2. Limpieza y Enriquecimiento
Durante la transformación, el script realiza las siguientes tareas críticas:
Normalización: Desanidado de diccionarios complejos de la API.
Ingeniería de Variables: Creación de la columna Densidad de Población (Población / Área).
Gestión de Nulos: Tratamiento de datos faltantes o incompletos.

3. Estructuración
Finalmente, los datos se cargan en un DataFrame de Pandas, permitiendo realizar:
✅ Análisis estadístico descriptivo.
✅ Agrupaciones por región o idioma.
✅ Visualizaciones gráficas.
✅ Muestreo de datos.

--- 

## EQUIPO 1:
📊 Proyecto Grupal de Estadística: Estadística descriptiva.
Nuestro análisis se ha centrado en los países europeos, escogiendo marcadores como densidad poblacional, área de los países y lenguaje para, a través de ellos, mostrar de una forma práctica como realizar consultas de estadística descriptiva (media, mediana, moda, varianza, desviación típica, percentil y cuartil).Proyecto Grupal de Estadística: Estadística descriptiva.
Nuestro análisis se ha centrado en los países europeos, escogiendo marcadores como densidad poblacional, área de los países y lenguaje para, a través de ellos, mostrar de una forma práctica como realizar consultas de estadística descriptiva (media, mediana, moda, varianza, desviación típica, percentil y cuartil).

- [Cheyenne](https://github.com/cheyennecg)
- [Jenireé](https://github.com/JenireeTovar)
- [Eva](https://github.com/evaponton)
- [Alex P.](https://github.com/AlexPG14)
- [Chiara](https://github.com/chiaracont)
- [Arantxa Sacacia](https://github.com/Aran87)

## EQUIPO 2:

<p>En éste ejercicio los diferentes grupos tendrán que consultar una API gratuita "Restcountries". Proporciona información detallada sobre todos los paises del mundo en un formato fácil de leer para los ordenadores (JSON).
Básicamente, es una gran base de datos pública a la que puedes "hacerle preguntas" a través de una URL.
El trabajo del **Grupo II** consiste en distinguir las diferentes gráficas y espicificar su uso más recomendado.

El grupo II está formado por:

- [***Sara Bailón***](https://github.com/Sara89359)            
- [***Arantxa Puig***](https://github.com/ArantxaPuig)        
- [***Fran Díaz***](https://github.com/FranDiazBusto)        
- [***Ágata Szlufcik***](https://github.com/AgataSzlufcik)        
- [***Juan G.***](https://github.com/xuangfm)    
- [***Julia***](https://github.com/Julia509-coll)    
  
<h2><center>Librerias usadas</h2></center>
Para éste proyecto se usaron las siguientes librerias:  
- **requests** *para hacer peticiones a la API*          
- **numpy** *para cáculos numéricos*          
- **pandas** *para crear y manejar el DataFrame*          
- **matplotlib** *para gráficas básicas*            
- **seaborn** *para gráficas más visuales*            
- **squlite3** *para poder crear y manejar bases de datos*          
- **scipy** *para estadística y pruebas de hipótesis*            
*Éste archivo, fué probado y desarrollado con las siguientes versiones de las librerías, para evitar posibles errores aconsejamos la instalación de ellas.*
pip install  requests==2.33.0 numpy==2.4.3 pandas==3.0.1 matplotlib==3.10.8 seaborn==0.13.2 scipy==1.17.1
*Recomendamos crear un entorno virtual para la ejecución del ejercicio*

## EQUIPO 3:

# 🎲 Probabilidad y distribuciones

### Probabilidad

La probabilidad mide el grado de incertidumbre de un evento. En el análisis de datos, permite estimar qué tan probable es obtener un determinado resultado, generalmente a partir de una pregunta o hipótesis planteada.

### Distribuciones
Las distribuciones describen cómo se reparten los valores o probabilidades de una variable, mostrando qué resultados son más o menos probables.

- [Graciela](https://github.com/Graceila82)
- [Krolina](https://github.com/KrolinaTF)
- [Diana](https://github.com/MiniiNa)
- [Alain](https://github.com/Alain-coder1)
- [Oksana](https://github.com/ksu727096-maker)
- [Francisco](https://github.com/fcoxjp-art)

Usamos datos para evaluar hipótesis bajo incertidumbre y tomar decisiones basadas en probabilidad.

## EQUIPO 4:

📊 Proyecto Grupal de Estadística: Correlación y Regresión

El núcleo de nuestro análisis consiste en entender cómo se relacionan el área de un país y su población. Para ello, utilizamos una muestra de 100 países elegidos de forma aleatoria, extraídos de una población total de 250 países.# Integrantes del equipo:

- [Jose](https://github.com/josepuges)
- [Lucía Llaneza](https://github.com/luciallaneza/luciallaneza)
- [Michelle](https://github.com/michelleolivares86-tech)
- [Alejandro](https://github.com/alexrey08)
- [Iván](https://github.com/Asenjo76/) 
- [Lucía Peláez](https://github.com/lucypelaez)

Enlace a GitHub: https://github.com/Asenjo76/Proyecto-grupal-Newton
