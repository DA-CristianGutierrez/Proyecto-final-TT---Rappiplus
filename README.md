# Proyecto-integral-Rappiplus

El dataset landing_experiment incluye 40.000 registros de usuarios únicos que se registraron en una de las dos versiones de la plataforma de Rappi.
En este proyecto se utilizaron varios datasets los cuales se unificaron tanto en python como en relaciones de modelados de datos, sin embargo, teniendo como base tabla el dataset orders_clean.csv el cual contiene 25.000 registros únicos (después de limpieza), events / users / user_activity, para analizar el comportamiento del funel y cohortes de usuarios dentro de la plataforma y experiment_checkout_ui.csv para evaluar diferencias de conversión entre dos versiones de grupos de compra.

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

# Resumen

En este proyecto aplique varias técnicas de análisis según requerimiento; inicialmente un cálculo de métricas generales para introducir una vista a la rentabilidad del negocio utilizando python. Construí funnels de cantidad y conversión de usuarios así como una matriz de cohortes con SQL. Apliqué un experimento A/B para comparar versiones de la plataforma. Finalmente tomé los datasets limpios para construir un análisis visual compuesto por dashboards que permitirían hacer un zoom a la rentabilidad a detalle creando segmentaciones. Como resultado, identifiqué puntos clave de mejora como en la tabla por cohortes, meses donde las ventas son críticas, así como inconsistencias en una de las etapas del funnel. 

## 🧠 Objetivo del análisis

Entender el desempeño del servicio y detectar oportunidades concretas de mejora.

## 🛠️ Herramientas y analisis aplicado:

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge&logo=matplotlib&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)

ETL, funnel de conversión, experimento A/B, análisis estadístico 

## Metodología

- Limpieza y transformación de datos: Se convirtieron tipos de dato al formato correcto, eliminaron duplicados, se estandarizaron categorías y finalmente se remplazaron valores nulos.
- Ejecución del análisis: Se ejecutaron los cálculos clave tales como métricas de negocio, funnel de retención y por cohortes, aplicación de pruebas estadísticas (experimento A/B). 
- Segmentaciones clave: Se construyeron dashboards para complementar el análisis previo con visualizaciones, así como la inclusión de segmentaciones clave. 


## Visualizaciones destacadas

1. Dashboard ejecutivo: Esta visualización contiene el orden de presentación estándar, ubicando las métricas generales del negocio en la parte superior mostrando la rentabilidad. Seguidamente se observan dos gráficos temporales evidenciando el pico de ventas y meses críticos. Finalmente un gráfico que aporta información sobre segmentos con su nivel de ingreso y respectiva ganancia. 

<img width="1092" height="575" alt="Captura de pantalla (28)" src="https://github.com/user-attachments/assets/e33123a7-4579-42f6-af10-5ff853ed580f" />



----------------------------------------------------------------------------------------------------------------------------------------


2. Dashboard detallado: Esta visualización devuelve la lista de ordenes y cantidad de ventas de un producto seleccionado en el dashboard general. Se agregan dos filtros que pueden arrojar mayor detalle si es de preferencia del usuario / stakeholder.

<img width="1075" height="545" alt="Captura de pantalla (27)" src="https://github.com/user-attachments/assets/23f2d96c-cb90-4e3b-a72e-53ad372d84e3" />


## Conclusiones y recomendaciones

- conversión_add_payment Es el proceso en el cual se presenta mayor abandono de usuarios.
- Los usuarios vuelven a comprar y al agruparlos por cohortes se detectan diferencias en la eficiencia de fidelidad del cliente.
- La prueba estadística aplicada en el experimento A/B indica que no existe evidencia suficiente para afirmar que hay una diferencia real entre ambas versiones.

Acciones recomendadas:

- Revisar que inconvenientes se están presentando en el paso de método de pago o expandir los métodos para mejorar la tasa de conversión.
- Considerar un mayor volumen de inversión en productos que generan ganancias considerables y cuestan menos para que el profit final pueda mejorarse.
