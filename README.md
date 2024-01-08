# Herramienta Predictiva para Venta de Inmuebles de Segunda Mano en Madrid

## Objetivo
Desarrollar una herramienta innovadora que se adapte a las preferencias y expectativas de los usuarios para identificar las mejores ofertas inmobiliarias en Madrid.

## Descripción del Proyecto
Este repositorio documenta los pasos seguidos en la creación de un modelo predictivo destinado a facilitar la búsqueda de inmuebles que cumplan con los requisitos y capacidades de los usuarios.

### Parte 1: Extracción de Datos (Web Scraping)
Se detalla el procedimiento y el código empleado para extraer información de 9.996 anuncios de pisos en `https://www.yaencontre.com/venta/pisos/madrid/e-segunda-mano.com`. Se aborda el desafío de 2.403 anuncios duplicados y la variabilidad en la estructura de los anuncios.

### Parte 2: Preprocesamiento y Análisis Exploratorio de Datos (EDA)
Se realiza la limpieza de datos, incluyendo la eliminación de duplicados y la transformación de variables. Se crean variables dummy para 'Equipamientos' y se dividen 'Características' y 'Ubicaciones' en columnas separadas. Posteriormente, se realiza un EDA para evaluar la distribución y relevancia de las variables en relación al precio de los inmuebles.

### Parte 3: Preprocesamiento NLP
Se procesan las variables 'Títulos' y 'Descripciones' obtenidas durante el scraping, realizando un análisis de frecuencia de palabras para identificar patrones comunes en los anuncios.

### Parte 4: Modelos de Regresión y Evaluación
Se entrena y evalúa tres modelos de regresión: Regresión Lineal, XG Boost y Random Forest. Se optimizan los modelos mediante escalado de datos y Grid Search. Se utilizan métricas como MSE, R2_Score y MAPE (Mean Absolute Percentage Error) para medir el rendimiento.

### Parte 5: Análisis de Outliers
Se reduce la cantidad de datos eliminando outliers, estableciendo un precio máximo de 950.000€ (75% del rango de precios) para evaluar su impacto en el rendimiento del modelo.

### Visualización de Resultados
Se presentan gráficos comparativos para ilustrar los resultados obtenidos con y sin la inclusión de outliers.

## Archivos y Código
Todos los códigos utilizados se importan desde un archivo externo que contiene las funciones empleadas en cada etapa del proyecto.
