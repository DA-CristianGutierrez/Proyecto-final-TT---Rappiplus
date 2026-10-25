# Proyecto-final-Rappiplus

Proyecto de análisis para Rappiplus
Este repositorio contiene el análisis combinado de limpieza de datos, funnels de conversión y retención por cohortes (conexión con SQL), aplicación de pruebas estadísticas y finalmente, presentación visual de negocio mediante herramienta Tableu.

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

## 🧠 Objetivo del análisis

- Revisar calidad y limpieza de datos
- Entender donde se pierden los usuarios y si regresan
- Determinar diferencias de compra entre dos versiones de grupos
- Crear visualizaciones que respondan las preguntas de negocio
