# Análisis de Fraude de Tarjetas de Crédito
En este análisis de fraude con tarjetas de crédito se investigan patrones ocultos mediante el cruce de datos geográficos y tipos de transacciones fraudulentas. 

## Adaptación de los datos
Este análisis está basado en el dataset de transacciones fraudulentas de [Machine Learning Group](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?resource=download).

El problema fue que estas transacciones estaban pensadas para ser procesadas a través de procesos de Machine Learning (lo cual no era mi objetivo), por lo tanto, decidí adaptar el dataset para hacerlo más interesante y poder analizar más a fondo las cualidades de este.
Al adaptar el dataset, he podido identificar tendencias y anomalías que revelan cómo y dónde ocurren estos fraudes, abriendo la puerta a un análisis detallado y estrategias preventivas futuras.

## Proceso de Transformación y Análisis del Dataset

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

### 5. **Análisis Exploratorio de Datos (EDA)**
   (Próximamente)

## Actualizaciones Futuras
Este proyecto está en desarrollo continuo. En futuras actualizaciones, se incluirán análisis más avanzados, como la segmentación de clientes, detección de patrones fraudulentos y visualizaciones adicionales que profundicen en los insights obtenidos.

## Conclusión
Este repositorio representa el comienzo de un análisis en profundidad de los datos de fraude con tarjetas de crédito. La cuidadosa adaptación del dataset es un paso crucial para garantizar que los análisis sean precisos y útiles desde una perspectiva analítica, en lugar de puramente predictiva.
