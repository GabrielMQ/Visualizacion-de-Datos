# DESAFÍO ALURA LATAM PYTHON PARA DATA SCIENCE - Visualización de datos

Presentado por: **Gabriel Enrique Montes Lambis**

Año: 2025

## Descripción del Contexto

Para la presentación de este challenge, he decidido usar un dataset obtenido de la plataforma GitHub [CÓDIGO BASE](https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_1%20.csv), que contiene los datos estadísticos de diferentes porcentajes de 4 tiendas pertenecientes al Sr. Juan.

La fuente de datos de este ejercicio se encuentra en *un repositorio*, para que su carga sea más simple al momento de la validación. El archivo usado se puede encontrar en:

### Importación de Datos

- Para tienda 1  ➡️ url1 "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_1%20.csv"
- Para tienda 2  ➡️ url2 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_2.csv"
- Para tienda 3  ➡️ url3 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_3.csv"
- Para tienda 4  ➡️ url4 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_4.csv"

Para permitir que la fuente de datos sea cargada desde la Libreria Pandas ®  Numpy & Matplotlib, fué necesario que el archivo tuviera permisos de lectura para "cualquiera con el link". 

## Contenido de la Actividad

En este análisis, se examina la situación del Señor Juan, quien debe tomar la importante decisión de qué tienda de las cuatro que posee debe vender para financiar un nuevo emprendimiento nuevo. El proyecto emplea un análisis de datos en Google Colab con Python para señalar la tienda con el rendimiento menos óptimo y proporcionar recomendaciones sólidas que faciliten su decisión.

Para obtener los resultados esperase se emplearon 5 pasos que son:

- 🛒 **Producto y Facturación**: Identificación del artículo vendido.
- 👨‍💻 **Categoría**: Clasificación del producto.
- 💯 **Calificación del Cliente**: Opinión del cliente sobre la experiencia de compra.
- 📅 **Frecuencia de Compra por catgoria**: Registro temporal y moda de la compra.
- 🚌 **Precio y Envío**: Costo de envío por transacción.




## 1. Análisis 

Se realiza un procedimiento de analisis e interpretación de datos siguiendo los pasos previamente definidos. 

## 1.1 Facturación

Se realizó un análisis de la facturación de las 4 tiendas, sumando los precios de los productos vendidos en cada una. Los resultados se muestran a continuación:

| Tienda  | Precio        |
|---------|---------------|
| Tienda 1| 1,150,880,000 |
| Tienda 2| 1,116,344,000 |
| Tienda 3| 1,098,020,000 |
| Tienda 4| 1,038,376,000 |

Además, se generó un gráfico de líneas para visualizar la facturación de cada tienda con lo cual se pudo dictaminar que la tienda 4 es la de menos facturación historica.

## 1.2 Ventas por categoria

Como segundo paso se realiza un análisis y visualización de datos de ventas de tiendas. Primero, se prepara los datos creando una lista de tuplas de categoría de producto y precio, y luego identifica las categorías únicas de productos. Tambiien se define Define una función (categoria_contador) para contar la frecuencia de cada categoría en cada tienda. Después, calcula y almacena estos conteos en un diccionario (resultados_categorias), donde las claves son los nombres de las tiendas. Finalmente, utiliza matplotlib para generar un gráfico de barras agrupadas que compara la cantidad de artículos por categoría entre las tiendas, facilitando la visualización de las diferencias en la distribución de productos.

## 1.3 Calificación promedio de la tienda

Se determina que tienda tiene menor y cual la mayor calificación, sienda la mayor la que obtuvo mayor satifacción.

## 1.4 Productos más y menos vendidos

En este paso se pretende analizar la distribución de categorías de productos en cuatro tiendas. Primero, identifica las categorías únicas de productos. Luego, define una función para contar cuántos productos pertenecen a cada categoría en una tienda dada. Aplica esta función a los datos de cada tienda y almacena los resultados en un diccionario. Finalmente, utiliza matplotlib para generar cuatro gráficos de pastel, uno por tienda, que visualizan la proporción de cada categoría de producto, permitiendo comparar fácilmente qué categorías son más o menos frecuentes en cada una.

- Tienda 1: Electrónicos: 24%, Muebles: 18%, Deportes y diversión: 16%, Electrodomésticos: 14%, Juguetes: 10%, Artículos para el hogar: 8%, Instrumentos musicales: 6%, Libros: 4%.

- Tienda 2: Electrónicos: 24%, Muebles: 18%, Juguetes: 16%, Electrodomésticos: 14%, Deportes y diversión: 10%, Artículos para el hogar: 8%, Instrumentos musicales: 6%, Libros: 4%.

- Tienda 3: Muebles: 24%, Electrónicos: 18%, Deportes y diversión: 16%, Electrodomésticos: 14%
Juguetes: 10%, Artículos para el hogar: 8%, Instrumentos musicales: 6%, Libros: 4%.

- Tienda 4: Electrónicos: 24%, Muebles: 18%, Juguetes: 16%, Deportes y diversión: 14%, Electrodomésticos: 10%, Artículos para el hogar: 8%, Instrumentos musicales: 6%, Libros: 4%.

## 1.5 Envío promedio por tienda

El código calcula y compara el costo promedio de envío entre cuatro tiendas. Primero, asigna los datos de cada tienda a variables separadas y luego calcula el costo promedio de envío para cada una. Utiliza matplotlib y seaborn para generar un gráfico de líneas que visualiza estos costos promedio, facilitando la comparación entre las tiendas. El gráfico incluye marcadores, etiquetas y anotaciones para mostrar claramente los costos de envío de cada tienda.

## 2. Recomendaciones 🗣️

El Sr. Juan debería vende la tienda 4 o 1, en caso de no poder conservar los costos de envio indudablemente debe vender la Tienda 4 primordialmente✅.

