# 🌤️ Comparador de Clima

Este proyecto es una herramienta interactiva en Python que permite consultar, comparar y visualizar datos climáticos históricos de diferentes ciudades y meses del año. Está pensado como parte de una consultoría climática enfocada en mostrar tendencias y comparaciones relevantes para usuarios o entidades interesadas en el análisis meteorológico.

## 🧰 Tecnologías utilizadas

- Python 3.12.3 
- Pandas
- Matplotlib

## 📁 Estructura del dataset

El archivo de datos debe tener la siguiente estructura (columnas):

- `Fecha`: Fecha de la medición (en formato datetime), pero de todas formas se valida si esta en un formato correcto en el archivo de ejemplo la fecha estuvo en formato d/m/y
- `Ciudad`: Nombre de la ciudad
- `Temperatura Maxima`
- `Temperatura Minima`
- `Precipitacion`
- `Velocidad del Viento`
- `Humedad Relativa`

## 🚀 Funcionalidades

### 🔍 Consultor de clima
Permite al usuario seleccionar una ciudad y un mes, y visualizar un gráfico de la temperatura máxima y mínima a lo largo del mes.

### 📊 Comparador climático
El usuario puede seleccionar **dos ciudades** y un **mes específico** para visualizar cinco gráficos comparativos:
- Temperatura máxima promedio
- Temperatura mínima promedio
- Precipitación total
- Humedad relativa promedio
- Velocidad del viento promedio

## 🧱 Organización del código

- `comparar_clima()`: Función principal de interacción para comparar ciudades.
- `crear_graficos(lista_ciudades, informacion, mes)`: Genera los gráficos comparativos.
-`calcular_metricas(df_ciudad)`: Función que los cálculos por ciudad segun el dataframe.

## 💡 Requisitos

Instala las dependencias con:

```bash
pip install pandas matplotlib
