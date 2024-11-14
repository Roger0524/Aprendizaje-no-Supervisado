# Hierarchical Clustering

Contiene la implementación de un modelo de clustering jerárquico, utilizado para segmentar clientes en función de variables como "Ingreso Anual" y "Puntaje de Gasto". La segmentación resultante proporciona información detallada sobre los distintos patrones de gasto y preferencias de los clientes.

## Descripción del Modelo

El modelo utiliza el método de enlace de Ward para maximizar la homogeneidad interna y la heterogeneidad entre clústeres. Con el dendrograma, se observó que cinco clústeres proporcionaban la mejor segmentación de los datos.

### Principales Métricas del Modelo

- **Coeficiente de Silhouette**: 0.62. Este valor indica una adecuada cohesión interna y separación entre clústeres, lo que permite que cada grupo refleje distintos comportamientos de los clientes.
- **Índice de Calinski-Harabasz**: 175.8. Este índice confirma que los clústeres son compactos y están bien diferenciados entre sí.

### Interpretación de los Resultados

La segmentación permite identificar diversos perfiles de cliente, tales como:
- Clientes de alto ingreso (>$100k) y alto puntaje de gasto (>80), que representan un segmento con alta capacidad de consumo.
- Clientes con ingresos medios ($40k-$80k) y puntajes de gasto moderados, que podrían beneficiarse de campañas de fidelización específicas.

Esta información ayuda a orientar campañas de marketing más personalizadas y mejorar la retención de clientes en función de sus patrones de gasto e ingreso.

## Requisitos

- Python 3.x
- Librerías: `numpy`, `pandas`, `scipy`, `scikit-learn`, `matplotlib`

## Uso

Para ejecutar el modelo, abre el archivo `Hierarchical.ipynb` en Jupyter Notebook o ejecuta el script en formato `.py`. Sigue las instrucciones para ajustar los parámetros y visualizar los resultados en un dendrograma y gráficos de dispersión.

## Visualización de Resultados

El modelo proporciona un dendrograma que permite visualizar la estructura jerárquica de los clústeres, y un gráfico de dispersión que ilustra la segmentación en función de "Ingreso Anual" y "Puntaje de Gasto".
