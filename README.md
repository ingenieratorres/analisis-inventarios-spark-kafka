# Análisis de datos para mejorar la gestión de inventarios mediante Apache Spark y Kafka

## 1. Descripción del proyecto

Este proyecto analiza datos históricos de ventas para identificar productos con mayores cantidades vendidas y observar su comportamiento a lo largo del tiempo. El propósito es explorar cómo las herramientas de Big Data pueden aportar información útil para apoyar la gestión de inventarios.

## 2. Conjunto de datos

Se utiliza el conjunto de datos **Online Retail**, publicado en el repositorio de la University of California, Irvine (UCI).

Fuente: https://archive.ics.uci.edu/dataset/352/online+retail

Los datos contienen información de transacciones comerciales, incluyendo códigos y descripciones de productos, cantidades, precios y fechas de facturación.

## 3. Herramientas utilizadas

- Python.
- Apache Spark mediante PySpark.
- RDD y DataFrames para el procesamiento y análisis de datos.
- Apache Kafka para la simulación de eventos.
- Spark Structured Streaming para consumir y procesar los eventos.
- Pandas y Matplotlib para apoyar la preparación y visualización de resultados.
- Google Colab como entorno de ejecución.

## 4. Procesamiento por lotes

El procesamiento incluye la carga de los datos, la revisión de su calidad, la eliminación de registros duplicados, la limpieza de transacciones no válidas y el análisis de las cantidades vendidas por producto y por mes.

Los resultados se presentan mediante tablas y gráficas para facilitar la interpretación de los datos.

## 5. Procesamiento con Kafka y Spark Streaming

Se configura un topic en Kafka y se generan eventos de ventas simulados. Spark Structured Streaming consume los eventos y permite calcular indicadores, como las unidades registradas y el valor simulado de las ventas.

Los eventos utilizados en esta práctica son simulados y no representan transacciones reales en tiempo real ni existencias actuales de inventario.

## 6. Archivo del proyecto

El repositorio incluye un cuaderno de Jupyter (`.ipynb`) con el código y los resultados guardados de la implementación.

## 7. Instrucciones generales de ejecución

1. Descargar o abrir el cuaderno del repositorio.
2. Abrirlo en Google Colab o en un entorno compatible con Python y PySpark.
3. Obtener el archivo Online Retail desde la fuente oficial indicada anteriormente y cargarlo en el entorno.
4. Ejecutar las celdas en orden.
5. Para la sección de Kafka y Spark Structured Streaming, preparar Java, Kafka y el conector de Spark Kafka según las instrucciones del cuaderno.

La ejecución puede requerir instalar dependencias y configurar los servicios antes de procesar los datos.

## 8. Resultados

El análisis permite identificar productos con altas cantidades vendidas, examinar tendencias mensuales y demostrar el procesamiento de eventos simulados mediante Kafka y Spark Structured Streaming.
