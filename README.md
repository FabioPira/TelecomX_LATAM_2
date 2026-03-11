readme = """
# TelecomX - Predicción de Cancelación de Clientes (Churn)

## Objetivo del Proyecto
El objetivo de este desafío es desarrollar modelos predictivos capaces de identificar clientes con alta probabilidad de cancelar sus servicios. Esto permite a la empresa anticiparse a la pérdida de clientes y diseñar estrategias de retención más efectivas.

---

## Desarrollo del Análisis

El proyecto se desarrolló siguiendo un pipeline típico de ciencia de datos:

1. **Limpieza y preparación de datos**
   - Corrección de tipos de datos
   - Eliminación de inconsistencias
   - Codificación de variables categóricas mediante One-Hot Encoding

2. **Análisis Exploratorio de Datos**
   - Identificación de patrones entre variables y churn
   - Análisis de correlación
   - Visualización de tendencias clave

3. **Modelado Predictivo**
   Se entrenaron dos modelos de clasificación:

   - Regresión Logística
   - Random Forest

   Los modelos fueron evaluados utilizando métricas como:
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - Matriz de Confusión

---

## Resultados del Análisis

### Relación entre permanencia del cliente y cancelación

![Tenure vs Churn](tenure_vs_churn.png)

Los clientes con menor tiempo en la empresa presentan mayor probabilidad de cancelar el servicio.

---

### Relación entre gasto total y cancelación

![Charges vs Churn](charges_vs_churn.png)

Los clientes que cancelan tienden a tener menor gasto acumulado, lo que indica cancelaciones tempranas.

---

### Matriz de correlación de variables

![Correlation Matrix](correlation_matrix.png)

El análisis de correlación permitió identificar variables relevantes para el modelado.

---

### Desempeño del modelo Random Forest

![Confusion Matrix RF](confusion_matrix_rf.png)

El modelo Random Forest mostró un mejor desempeño para identificar clientes con riesgo de cancelación.

---

## Conclusión

El análisis permitió identificar factores importantes asociados al churn, como el tiempo de permanencia del cliente, el tipo de contrato y el nivel de gasto. 

El modelo Random Forest mostró mayor capacidad para detectar clientes en riesgo de cancelación, lo que sugiere que los modelos basados en árboles pueden capturar mejor patrones complejos en los datos.

Estos resultados pueden ser utilizados por la empresa para implementar estrategias de retención dirigidas a clientes con mayor probabilidad de abandonar el servicio.
"""

with open("README.md", "w") as f:
    f.write(readme)

print("README.md generado correctamente")
