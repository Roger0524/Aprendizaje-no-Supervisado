# K-means Clustering

Contiene la implementación de un modelo de clustering K-means, utilizado para segmentar clientes en función de variables relevantes como el "Ingreso Anual" y el "Puntaje de Gasto". Este enfoque ayuda a identificar patrones de comportamiento en grupos de clientes, optimizando estrategias de marketing y personalización de servicios.

## Descripción del Modelo

El algoritmo de K-means organiza a los clientes en cinco clústeres, basándose en la variabilidad observada en los datos. La cantidad de clústeres fue determinada mediante el método del codo, que indicó que cinco era el número óptimo para capturar las diferencias entre clientes de manera eficaz.

### Principales Métricas del Modelo

- **Coeficiente de Silhouette**: 0.63. Este valor indica una segmentación adecuada, con cohesión interna en los clústeres y buena separación entre ellos.
- **Índice de Calinski-Harabasz**: 310. Un valor elevado que sugiere buena compactación interna y separación clara entre clústeres.

### Interpretación de los Resultados

La segmentación generada permite distinguir entre diferentes perfiles de cliente. Por ejemplo:
- Clientes con ingresos altos y puntajes de gasto bajos, indicando un comportamiento de gasto conservador.
- Clientes con ingresos moderados y puntajes de gasto altos, que podrían ser más propensos a consumir en productos del centro comercial.

Esta información puede ayudar a optimizar campañas de marketing y orientar promociones hacia los segmentos más interesados en determinados productos o servicios.

## Requisitos

- Python 3.x
- Librerías: `numpy`, `pandas`, `scikit-learn`, `matplotlib`

## Uso

Para ejecutar el modelo, simplemente corre el archivo `K-means.ipynb` en Jupyter Notebook o ejecuta el script correspondiente si está en formato `.py`. El archivo incluye las instrucciones para ajustar los parámetros y evaluar los resultados.

## Resultados y Visualización

Los resultados se presentan gráficamente, mostrando la distribución de los clústeres en un gráfico de dispersión de "Ingreso Anual" vs. "Puntaje de Gasto". Esto facilita la interpretación de los patrones de comportamiento de los clientes en función de su posición en cada clúster.
