# Proyecto-integral-Rappiplus

El dataset landing_experiment incluye 40.000 registros de usuarios únicos que se registraron en una de las dos versiones de la página.
En este proyecto se utilizaron varios datasets los cuales se unificaron tanto en python como en relaciones de modalados de datos, sin embargo, teniendo como base tabla el dataset orders_clean.csv el cual contiene 25.000 registros únicos (después de limpieza), events / users / user_activity, para analizar el comportamiento del funel y cohortes de usuarios dentro de la plataforma y
experiment_checkout_ui.csv para evaluar diferencias de conversión entre dos versiones de grupos de compra.

## 📂 Contenido del repositorio

- `s12_estudiante_proyecto_final.ipynb`
  → Notebook principal con limpieza, analisis de conversión y retención de usuarios, aplicación de prueba estadística.
  
- `Dashboard proyecto Rappiplus- Tableu.twb`
  → Dashboard con cálculo de métricas para respuestas de negocio utilizando los datasets limpios del notebook principal.
  
## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DA-CristianGutierrez/Proyecto-final-TT---Rappiplus/blob/main/s12_estudiante_proyecto_final.ipynb)

o:

1.Abre el archivo .ipynb en GitHub

2.Haz clic en Open in Colab

## 📘 Cómo reproducir el análisis

1.Abre `s12_estudiante_proyecto_final.ipynb`
2.Ejecuta las celdas en orden
3.El notebook carga automáticamente el dataset desde /data/ o desde un enlace público (según corresponda)

## Análisis integral RappiPlus

En este proyecto aplique varias técnicas de análisis requeridas por la necesidad del negocio; inicialmente un cálculo de métricas generales para introducir una vista a la rentabilidad del negocio utilizando python. Construí funnels de cantidad y conversión de usuarios así como una matriz de cohortes con SQL. Apliqué un experimento A/B para comparar versiones de la plataforma. Finalmente tomé los datasets limpios para construir un análisis visual compuesto por dashboards que permitirían hacer un zoom a la rentabilidad a detalle del negocio creando segmentaciones. Como resultado, identifiqué puntos clave de mejora como en la tabla por cohortes, meses donde las ventas son críticas, así como inconsistencias en una de las etapas del funnel. 

## 🧠 Objetivo del análisis

Entender el desempeño del servicio y detectar oportunidades concretas de mejora.

## 🛠️ Herramientas y analisis aplicado:

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge&logo=matplotlib&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)

ETL, funnel de conversión, experimento A/B, análisis estadístico 

## Metodología

- Limpieza y transformación de datos: Se realizó .
- Verificación clave: Se verificó que los registros tuvieran un identificador único y sin duplicados con el fin de evitar errores en la aplicación de las pruebas estadísticas.
- Aplicación de pruebas estadísticas: Se aplicaron las pruebas que determinan diferencias clave; promedios entre versiones, canales, tipos de usuarios.
- Segmentaciones clave: Se presentaron visualizaciones por segmentos clave para complementar y confirmar el analisis. 


## Visualizaciones destacadas

1. Gráfico conversiones por canal: La visualización indica claramente la fuente de tráfico más y menos usada por los usuarios así como una visual de conversión para cada fuente. La tasa de conversión es proporcional en todos los canales, lo cual indica que el proceso de compra es de la misma fluidez en cada canal.


<img width="589" height="455" alt="image" src="https://github.com/user-attachments/assets/a0333f25-5af2-45c1-9fa8-371b8d2628b3" />


----------------------------------------------------------------------------------------------------------------------------------------


2. Gráfico conversiones por tipo de usuario: Se evidencia una conversión proporcional entre ambos tipos de usuario, sin embargo, presenta diferencias significativas en el volumen de estos, lo cual arroja una clave en este segmento.

<img width="589" height="455" alt="image" src="https://github.com/user-attachments/assets/9163a4ea-d031-4e25-a06b-f49d8a014372" />


## Conclusiones y recomendaciones
- Prueba entre versiones A/B: La diferencia en la tasa de conversión entre ambas paginas es de aproximadamente 3 puntos porcentuales,  predominando en el grupo B la mayor tasa de conversión.
- Organic y ADS son las fuentes que más usuarios canalizan, sin embargo, la tasa de conversión es simétrica en todos las fuentes de trafico.
- Los usuarios nuevos generan mayor cantidad de conversiones, aunque nuevamente, la tasa de conversión se mantiene simétrica entre ambos grupos.

Acciones recomendadas:

- Revisar la diferencia de limitaciones entre las versiones de la página A y la página B así como el proceso de compra el cual es más efectivo en la página B.
- Revisar el stock de productos buscados por usuarios recurrentes donde haya mayor coincidencia para generar promociones o incluso entender que están buscando realmente para incrementar la probabilidad de compra.
