
🌏 Proyecto de Análisis: REST Countries API
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
🛠️ Procesamiento y Transformación
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
python
import pandas as pd

# El resultado final es un objeto df listo para la acción:

df = pd.DataFrame(rows)

📊 Proyecto Grupal de Estadística: Correlación y Regresión

---
El núcleo de nuestro análisis consiste en entender cómo se relacionan el área de un país y su población. Para ello, utilizamos una muestra de 100 países elegidos de forma aleatoria, extraídos de una población total de 250 países.

--- 

1. 📈 Correlación¿Están relacionados? ¿Cómo de fuerte es esa relación?

Lo primero que hicimos fue medir la Correlación de Pearson, obteniendo un valor de $r = 0.54$. Esto indica una relación positiva moderada: por lo general, a mayor área, mayor población.Sin embargo, al aplicar la correlación de Spearman, el valor subió a 0.91. Esto demuestra que la relación es mucho más fuerte de lo que parece, pero no es lineal debido a los "países gigantes" o muy "pequeños" (valores atípicos o outliers).

---


2. 📏 Regresión Lineal¿Podemos predecir?

Con la regresión, intentamos trazar la "línea perfecta" que atraviesa nuestros datos. Creamos una fórmula matemática que nos permite estimar: "Si un país mide $X$ área, su población debería ser $Y$ habitantes".
Ejemplo: Nuestro modelo predice que para un país de $100 \text{ km}^2$, la población esperada es de unos 76 habitantes.

---

3. ✅ Bondad de Ajuste ($R^2$)¿Es fiable el modelo?

Aquí medimos la calidad del ajuste. Nuestro $R^2$ es de 0.30, lo que significa que el tamaño del territorio explica el 30% de la variación de la población. El otro 70% depende de factores externos como la economía, el clima o la historia. El área no lo es todo.

---

4. 🔍 Residuos y Error¿Dónde fallamos?

Los residuos son la diferencia entre la predicción del modelo y la realidad. Estudiar el error es vital porque nos avisa que no podemos aplicar la misma regla a todos por igual.

---

Tipo de Residuo y 📝 Significado:

📍 EjemploPositivo ➕El país tiene más población de la que le "correspondería" por su tamaño.Países densos (Singapur, India).

Negativo ➖El país tiene menos población de la que se esperaría para su extensión.Países con desiertos o zonas polares (Canadá).

Cero 🎯Predicción perfecta. El país se comporta exactamente según la tendencia global.Caso ideal.

## EQUIPO 1:


## EQUIPO 2:


## EQUIPO 3:


## EQUIPO 4:

En nuestro equipo nos hemos encargado de investigar correlacion-regresion, (dirección e intensidad). Regresión lineal simple. Interpretación básica de R2 y error. 
Integrantes del equipo:
- [Jose](https://github.com/josepuges)
- [Lucía Llaneza](https://github.com/luciallaneza/luciallaneza)
- [Michelle](https://github.com/michelleolivares86-tech)
- [Alejandro](https://github.com/alexrey08)
- [Iván](https://github.com/Asenjo76/) 
- [Lucía Peláez](https://github.com/lucypelaez)

Enlace a GitHub: https://github.com/Asenjo76/Proyecto-grupal-Newton
