# Exploración y Visualización de Datos con D3.js
Práctica de Exploración y Visualización de Datos con D3 del _Bootcamp Big Data & Machine Learning_ de [KeepCoding](https://keepcoding.io/es/).

## Objetivo
Esta práctica tiene como ojetivo desarrollar un pequeño dashboard mediante el uso de librería **D3.js**. El dahsboard se compone de tres gráficas que representarán:
1. Un mapa con los barrios de madrid, donde los colores indiquen el precio medio de alquiler por barrio.
1. Una gráfica para visualizar cuántas propiedades hay en función del número de habitaciones.
1. Una gráfica donde se muestre el precio del alquiler frente al número de habitaciones, además de una recta que respresente la regresión lineal calculada a partir de estos puntos.

Las dos gráficas mostrarán la información relativa al barrio seleccionado en el mapa superior.

### Dataset
El dataset utilizado es un fichero json adaptado para la práctica, con informacion geogragráfica de los barrios en formato geojson junto con la información necesaria para el resto de gráficas.

## Desarrollo
La página web desarrada consta de varios ficheros:
- index.html: página principal, con la estructura para cargar los gráficos
- main.css: hoja de estilos para definir la estructura de la página y colores de los gráficos.
- map-d3-leaflet.js: son las funciones de javascript programadas para leer los datos, y repesentarlos haciendo uso de la librería _d3.js_.  
A continuación se muestra una captura donde se pueden visualizar los tres gráficos del dashboard desarrllado.

![dashboard](img/web.png)

1. La visualización del mapa de _d3.js_ se ha integrado con la librería _Leaflet_, con el ojetivo de poder visualizar un mapa base junto con el de barrios de Mardrid (en nuestro caso un mapa proporcionado por CartoDB)
1. Las gráficas 2 y 3 se actualizan con la información relativa a un barrio, seleccionandolo al pasar el puntero por por encima de uno de los barrios del mapa superior. El eje Y (del gráfico 2) es dinámico para permitir visualizar mejor los valores, sin embargo, en el caso de la gráfica de la Regresion Lineal se ha mantenido estático para que se puedan comparar mejor las rampas de la RL entre distintos barrios.

## Estudio y Dudas

## Referencias
Algun de las páginas consultadas para el desarrollo de la práctica han sido:
- 
