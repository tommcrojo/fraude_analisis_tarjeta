# Análisis de Fraude de Tarjetas de Crédito
En este análisis de fraude con tarjetas de crédito se investigan patrones ocultos mediante el cruce de datos geográficos y tipos de transacciones fraudulentas. 

## Adaptación de los datos
Este análisis está basado en el dataset de transacciones fraudulentas de [Machine Learning Group](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?resource=download).

El problema fue que estas transacciones estaban pensadas para ser procesadas a través de procesos de Machine Learning (lo cual no era mi objetivo), por lo tanto, decidí adaptar el dataset para hacerlo más interesante y poder analizar más a fondo las cualidades de este.
Al adaptar el dataset, he podido identificar tendencias y anomalías que revelan cómo y dónde ocurren estos fraudes, abriendo la puerta a un análisis detallado y estrategias preventivas futuras.

## 🔨 Proceso de Transformación 

### 1. **Exploración Inicial del Dataset**
   - **Carga de Datos:** Comencé cargando el dataset y realizando una exploración inicial para entender la estructura y el contenido de los datos.

### 2. **Limpieza de Datos**
   - **Manejo de Valores Faltantes:** Identifiqué y manejé valores faltantes dentro del dataset, aplicando técnicas como la imputación o la eliminación de filas/columnas según fuera necesario.
   - **Corrección de Errores:** Revisé y corregí errores en los datos, asegurándome de que todos los campos estuvieran en un formato consistente y adecuado para el análisis.

### 3. **Transformación de Variables**
   - **Normalización y Escalado:** Algunas variables fueron normalizadas o escaladas para mejorar la interpretabilidad y la comparabilidad entre distintas características.
   - **Codificación de Variables Categóricas:** Las variables categóricas se codificaron utilizando técnicas adecuadas (como la codificación one-hot) para preparar los datos para su análisis.

### 4. **Creación del DataFrame Final**
   - **Consolidación de Transformaciones:** Todas las transformaciones y limpiezas realizadas se consolidaron en un nuevo DataFrame, optimizado para el análisis posterior.
   - **Verificación de Integridad:** Realicé verificaciones adicionales para asegurar que el DataFrame final estaba libre de errores y era coherente con los objetivos del análisis.

![image](https://github.com/user-attachments/assets/967de6ce-c9bc-4103-9f50-8787d9912ca2)

## 🔎 Identificación de Fraudes

Con esta sección buscamos identificar transacciones sospechosas en un conjunto de datos utilizando técnicas de análisis de datos con Python. Las librerías utilizadas incluyen pandas, numpy, matplotlib y seaborn.

Pasos Realizados:

### Importación de Librerías:
Se importaron las librerías necesarias para el análisis de datos y la visualización.

### Carga del DataFrame:
Se cargó el DataFrame con los datos de transacciones.

### Conversión de la Columna de Tiempo:
Se convirtió la columna de tiempo a formato datetime para facilitar el análisis temporal.

### Creación de la Columna possible_fraud:
Se creó una nueva columna possible_fraud para marcar las transacciones sospechosas.

### Identificación de Transacciones en Altas Horas de la Noche:
Se identificaron transacciones realizadas entre las 2am y las 5am, marcándolas como posibles fraudes.

### Identificación de Transacciones de Grandes Cantidades:
Se calcularon los umbrales para grandes cantidades utilizando el percentil 99.5 y se marcaron las transacciones que superan este umbral como posibles fraudes.

### Identificación de Transacciones Inusuales para Cada Usuario:
Se calcularon la media y la desviación estándar de las transacciones de cada usuario.

Se identificaron transacciones que se desvían significativamente de la media del usuario (más de 5 desviaciones estándar) y se marcaron como posibles fraudes.

### Visualización de Outliers:
Se crearon gráficos para visualizar las transacciones sospechosas, incluyendo un gráfico de pastel para mostrar el porcentaje de transacciones marcadas como posibles fraudes frente a las que no lo están.

### 🧠 Resultados
Porcentaje de Transacciones Marcadas como Posible Fraude:
Se observó que aproximadamente el 17% de las transacciones fueron marcadas como posibles fraudes. Este porcentaje es más alto de lo esperado debido a que los datos utilizados son sintéticos y generados de forma aleatoria, lo que puede introducir anomalías no representativas de un conjunto de datos real.
![image](https://github.com/user-attachments/assets/fccbcb7b-8375-4ee1-8984-dd39bb0966e4)

## 📊 Visualización de datos

Dashboard en PowerBI:
![image](https://github.com/user-attachments/assets/18231846-6d8e-47d8-b675-5b8575016c8a)
Si quieres interactuar con el dashboard, puedes descargar este archivo en la carpeta


## Conclusión
Este repositorio representa el comienzo de un análisis en profundidad de los datos de fraude con tarjetas de crédito. La cuidadosa adaptación del dataset es un paso crucial para garantizar que los análisis sean precisos y útiles desde una perspectiva analítica, en lugar de puramente predictiva.
