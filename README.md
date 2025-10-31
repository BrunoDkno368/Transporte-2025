# Transporte-2025
Cantidad de transacciones SUBE (usos) por día en 2025 datos reales de la secretaria de transporte actualizada hasta el 30/10/2025
📊 Análisis de Datos de Uso del Transporte Público en Argentina (2025)
🧩 Descripción del Proyecto

Este proyecto tiene como objetivo realizar un proceso completo de análisis de datos (ETL + EDA) utilizando información pública del Ministerio de Transporte de la Nación Argentina, específicamente sobre los usos de la tarjeta SUBE a nivel nacional.

El análisis busca identificar patrones de movilidad, tendencias de uso y distribución del transporte entre jurisdicciones, tipos de transporte, provincias y empresas prestatarias.

🧠 Objetivos

Aplicar un proceso ETL (Extract, Transform, Load) con datos reales.

Desarrollar un análisis exploratorio de datos (EDA) para comprender el comportamiento del transporte público.

Detectar tendencias temporales y geográficas.

Presentar visualizaciones claras que aporten valor al análisis.

Elaborar un dataset limpio y reutilizable para futuros proyectos de analítica o machine learning.

🧰 Tecnologías Utilizadas

Lenguaje: Python 🐍

Librerías:

pandas (procesamiento y limpieza de datos)

matplotlib (visualizaciones)

numpy

Fuente de Datos: Datos Abiertos del Ministerio de Transporte

Archivo Original: usos_transporte.csv

Archivo Resultante: datos_usos_2025_ETL.csv

⚙️ Proceso ETL
🔹 Extract

Se obtuvo el dataset original en formato .csv desde el portal de Datos Abiertos del Gobierno Argentino, con información de transacciones del sistema SUBE.

🔹 Transform

Durante esta etapa se realizaron las siguientes operaciones:

Normalización de tipos de datos:

Conversión de la columna DIA_TRANSPORTE de object a datetime64.

Creación de nuevas columnas:

MES (en texto) y DIA (día de la semana en español).

Tratamiento de valores nulos:

Reemplazo de valores faltantes por "Sin datos".

Homogeneización de nombres:

Reemplazo de abreviaciones (JN → Jurisdicción Nacional, CIUDAD AUTÓNOMA DE BUENOS AIRES → C.A.B.A.).

Estandarización de texto y categorías.

🔹 Load

Se generó un nuevo archivo limpio:

datos_usos_2025_ETL.csv

🔍 Análisis Exploratorio de Datos (EDA)

Se realizaron diversos análisis y visualizaciones para obtener información relevante:

📈 1. Distribución por tipo de transporte

Identifica cuáles medios de transporte concentran la mayor cantidad de transacciones.

![Presentación1](https://github.com/user-attachments/assets/f122658f-fc41-43b8-87e4-faee4e47efeb)


🏙️ 2. Interior vs AMBA

Comparativa del uso de transporte en el Área Metropolitana de Buenos Aires frente al interior del país.

🗺️ 3. Jurisdicciones y Provincias

Se analizaron las diferencias entre provincias y jurisdicciones, destacando aquellas con mayor volumen de pasajeros.


![Presentación3](https://github.com/user-attachments/assets/2e896fb4-61c6-4b91-8f1e-540933c0e467)

📆 4. Análisis temporal

Por Mes: muestra la evolución del uso del transporte a lo largo del año.

![Presentación2](https://github.com/user-attachments/assets/ec509c72-a34d-4b08-860f-675b5e5004cf)


Por Día de la Semana: permite identificar los días con mayor demanda.

🏢 5. Top 10 Empresas

Ranking de las empresas con mayor cantidad de transacciones registradas.

📊 Visualizaciones Clave

Algunas de las gráficas más relevantes generadas fueron:

Gráfico de barras horizontales por tipo de transporte.

Gráfico de torta para distribución AMBA vs Interior.

Barras por provincia con total de pasajeros.

Gráfico lineal de evolución mensual del transporte.

Top 10 de empresas con mayor cantidad de usos.

📈 Conclusiones Principales

El AMBA concentra el mayor uso del transporte público, lo que refleja la densidad poblacional y la centralidad económica de la región.

Los colectivos son el medio de transporte más utilizado, superando ampliamente a trenes y subtes.

La Jurisdicción Nacional y C.A.B.A. son los principales focos de transacciones, indicando una fuerte concentración del sistema SUBE.

El uso del transporte varía según el mes y día, mostrando caídas en fines de semana y aumentos en días hábiles.

El dataset demuestra ser una excelente base para análisis de movilidad, planificación urbana y subsidios al transporte.

💾 Archivos Generados
Archivo	Descripción
usos_transporte.csv	Dataset original descargado del portal de datos abiertos
datos_usos_2025_ETL.csv	Dataset limpio, normalizado y transformado
graficos/	Carpeta sugerida para guardar las visualizaciones generadas
README.md	Documento explicativo del proyecto
🚀 Próximos pasos

Incorporar análisis con series temporales para predecir demanda futura.

Explorar modelos de Machine Learning para detectar patrones de movilidad.

Crear un dashboard interactivo en Power BI o Streamlit.

🧑‍💻 Autor

Bruno Roberto Argañaraz
Analista de Datos
📍 Argentina
💼 LinkedIn  https://www.linkedin.com/in/bruno-argañaraz-726a4a199/
 | 🌐 GitHub
