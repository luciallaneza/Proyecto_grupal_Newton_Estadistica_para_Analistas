
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

## EQUIPO 2:

## EQUIPO 3:

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
