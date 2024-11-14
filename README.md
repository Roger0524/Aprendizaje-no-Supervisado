# Modelos de Clustering para "Customer Segmentation"

Este repositorio contiene dos modelos de clustering, **K-means** y **Jerárquico**, implementados para segmentar clientes basándose en sus características de "Ingreso Anual" y "Puntaje de Gasto". La segmentación permite identificar diferentes patrones de comportamiento, ayudando a crear estrategias de marketing y personalización de servicios más efectivas.

## Modelos Incluidos

1. **K-means Clustering**: Un modelo de clustering basado en particiones que divide a los clientes en clústeres disjuntos. Se seleccionaron cinco clústeres utilizando el método del codo. Este modelo es adecuado para identificar grupos de clientes que comparten características similares.

2. **Hierarchical Clustering**: Un modelo de clustering jerárquico que organiza los datos en una estructura anidada. El modelo utiliza el método de enlace de Ward, y la cantidad de clústeres se determinó como cinco, en función del dendrograma.

## Métricas de Evaluación

Ambos modelos se evaluaron con las siguientes métricas:

- **Coeficiente de Silhouette**: Mide la cohesión y separación de los clústeres. Valores cercanos a 1 indican buenos resultados de segmentación.
  - K-means: 0.63
  - Jerárquico: 0.62

- **Índice de Calinski-Harabasz**: Mide la densidad y separación de los clústeres. Valores altos sugieren una buena compactación y dispersión entre clústeres.
  - K-means: 310
  - Jerárquico: 175.8

## Aplicación de los Modelos

Estos modelos son útiles para crear estrategias de marketing dirigidas, tales como:
- Ofrecer promociones específicas a clústeres con alta probabilidad de consumo.
- Personalizar campañas de retención para clústeres con patrones de gasto moderados o bajos.
- Segmentar a clientes de alto ingreso y alto puntaje de gasto para ofrecerles servicios premium.

## Requisitos

- Python 3.x
- Librerías: `numpy`, `pandas`, `scikit-learn`, `scipy`, `matplotlib`

## Ejecución

Cada modelo puede ejecutarse en Jupyter Notebook:
- **K-means**: `K-means.ipynb`
- **Jerárquico**: `Hierarchical.ipynb`

Sigue las instrucciones dentro de cada notebook para ajustar los parámetros y evaluar los resultados.
