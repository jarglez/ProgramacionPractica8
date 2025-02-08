# Práctica 8: 

Elaboró: Carlos Alejandro Jarero Gonzalez <al255813@alumnos.uacj.mx>

Matrícula: 255813

El presente Notebook fue relizado en equipo local con Kernel Python 3.11.8 en VS Code.

## Objetivos

Este ejercicio tiene como objetivo que los estudiantes aprendan a trabajar con seaborn para crear visualizaciones más avanzadas utilizando gráficos como el mapa de calor y el diagrama de violín. También, se les anima a explorar el dataset, hacer análisis descriptivos y aprender a interpretar los resultados.

## Dataset:
En este caso, vamos a utilizar el dataset de "tips" de seaborn, que contiene información sobre las propinas que dejaron los clientes en un restaurante, junto con detalles sobre el total de la cuenta, el día de la semana, si fue almuerzo o cena, entre otros. Para ello, los estudiantes podran cargar el dataset de la siguiente forma

```python
import seaborn as sns 
df = sns.load_dataset('tips')
```
## Instrucciones

- Formato y personalización de los gráficos:
    - Personaliza cada gráfico con títulos, etiquetas en los ejes y leyendas cuando sea necesario.
    - Experimenta con diferentes colores, estilos y tamaños para hacer que las visualizaciones sean claras y atractivas.

1. Carga y exploración del dataset:

    - Cargar el dataset tips usando seaborn.
    - Realizar un análisis preliminar: utiliza ```.head()```, ```.info()```, ```.describe()``` para obtener una visión general de los datos.
    - Verificar la existencia de valores nulos o datos faltantes.

2. Crear los siguientes gráficos con Seaborn:

    a) Mapa de Calor (Heatmap):

    - Objetivo: Visualizar la correlación entre las variables numéricas en el dataset.
    - Instrucciones: Utiliza un mapa de calor para mostrar la matriz de correlación entre las variables numéricas (total_bill, tip, size).
    - Asegúrate de personalizar el mapa con una paleta de colores y etiquetas en los ejes.

    b) Diagrama de Violín:

    - Objetivo: Mostrar la distribución de las propinas (tip) para diferentes días de la semana.
    - Instrucciones: Utiliza un diagrama de violín para comparar cómo varía la distribución de las propinas en cada uno de los días (day).
    - Personaliza el gráfico con colores y etiquetas adecuadas.

    c) Gráfico de dispersión (Scatter Plot):

    - Objetivo: Analizar la relación entre el total de la cuenta (total_bill) y la propina (tip).
    - Instrucciones: Crea un gráfico de dispersión con total_bill en el eje X y tip en el eje Y. Usa un color diferente para cada día de la semana.

    d) Gráfico de barras (Bar Plot):

    - Objetivo: Comparar el promedio de la propina (tip) por género (sex).
    - Instrucciones: Utiliza un gráfico de barras para mostrar el promedio de las propinas por género (hombres y mujeres).