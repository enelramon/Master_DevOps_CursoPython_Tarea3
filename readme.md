# Trabajo 3: Análisis de datos con Numpy y Pandas - RetailNow

## Descripción
Este proyecto consiste en analizar los datos de ventas, inventarios y satisfacción del cliente para la cadena de tiendas minoristas ficticia "RetailNow". El objetivo es procesar, explorar y analizar estos datos utilizando Pandas y Numpy para ayudar a la dirección a tomar decisiones estratégicas orientadas a optimizar el rendimiento de las sucursales.

## Archivos del Proyecto
* **Archivo principal:** `analisis_red_tiendas.ipynb` (Jupyter Notebook donde se desarrollará todo el código).
* **Datos requeridos (CSV):** 
  * `sales.csv`: Datos de ventas.
  * `inventories.csv`: Datos de inventarios.
  * `satisfaction.csv`: Datos de satisfacción de clientes.

## Pasos a Seguir

### 1. Preparación e Importación
* Prepara tu entorno en Visual Studio Code con el plugin de Jupyter.
* Importa las librerías `pandas` y `numpy`.

### 2. Carga y Procesamiento de Datos (Pandas)
* Carga los archivos CSV (`sales.csv`, `inventories.csv`, `satisfaction.csv`) en tres DataFrames distintos. Las rutas deben ser absolutas (ej. `/workspace/sales.csv`).
* Limpia los datos eliminando las filas con valores nulos utilizando el método `dropna()`.

### 3. Exploración de Datos (Pandas)
* Calcula las ventas totales por producto y por tienda.
* Calcula los ingresos totales por tienda (cantidad vendida × precio unitario).
* Genera un resumen estadístico de las ventas con el método `describe()`.
* Calcula el promedio de ventas por tienda y categoría de productos usando `groupby()`.

### 4. Análisis de Inventarios (Pandas)
* Calcula la rotación de inventarios para cada tienda dividiendo las ventas totales por el stock disponible y almacena el resultado en una nueva columna.
* Filtra e identifica las tiendas con niveles críticos de inventario (aquellas donde el porcentaje de productos vendidos sea menor al 10% del stock disponible).

### 5. Análisis de Satisfacción del Cliente (Pandas)
* Relaciona los datos de satisfacción con el rendimiento de ventas.
* Filtra las tiendas con niveles bajos de satisfacción (menor al 60%) para formular recomendaciones.

### 6. Operaciones y Simulaciones Numéricas (Numpy)
* Convierte la columna de ventas totales a un array de Numpy (usando `.to_numpy` o `.values`).
* Utiliza Numpy para calcular la **mediana** y la **desviación estándar** de las ventas totales.
* Utiliza el módulo de aleatoriedad de Numpy para generar arrays aleatorios que simulen proyecciones de ventas futuras. Asegúrate de establecer una semilla (`seed`) para la reproducibilidad.

## Requisitos Técnicos
* El código debe estar estructurado en un archivo Jupyter Notebook (`.ipynb`).
* El código debe estar correctamente organizado y comentado, explicando los pasos y análisis realizados.
* Se debe demostrar el uso explícito de Numpy para los cálculos estadísticos solicitados, aunque estos puedan realizarse en Pandas.

## Criterios de Evaluación
* **30% - Carga y manejo de datos (Pandas):** Carga correcta de los archivos CSV, limpieza de valores nulos y estructuración adecuada de los DataFrames.
* **30% - Análisis de datos (Pandas):** Cálculo correcto de ventas totales, rotación de inventarios, satisfacción del cliente, y aplicación correcta de filtros críticos (<10% inventario, <60% satisfacción).
* **20% - Cálculos estadísticos (Numpy):** Uso correcto de Numpy para calcular la mediana y la desviación estándar de las ventas.
* **20% - Simulación de datos (Numpy):** Generación de proyecciones de ventas futuras con arrays aleatorios y cálculo de estadísticas sobre dichas proyecciones.