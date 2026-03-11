# TelecomX - Predicción de Cancelación de Clientes

## Objetivo

Desarrollar modelos predictivos capaces de identificar clientes con alta probabilidad de cancelar sus servicios (churn), permitiendo a la empresa anticipar estrategias de retención.

---

## Desarrollo del Análisis

El proyecto se desarrolló siguiendo un pipeline de ciencia de datos:

1. **Preparación de datos**
   - Limpieza y transformación del dataset.
   - Conversión de tipos de datos.
   - Codificación de variables categóricas mediante **One-Hot Encoding**.

2. **Análisis exploratorio de datos**
   - Evaluación de correlaciones entre variables.
   - Identificación de patrones asociados a la cancelación de clientes.

3. **Modelado predictivo**

Se entrenaron dos modelos de clasificación:

- **Regresión Logística** (requiere normalización de variables).
- **Random Forest** (modelo basado en árboles, no sensible a escala).

Los datos se dividieron en:

- **80% entrenamiento**
- **20% prueba**

4. **Evaluación de modelos**

Los modelos fueron evaluados mediante las siguientes métricas:

- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusión

---

## Resultados

El modelo **Random Forest** presentó un mejor desempeño general al identificar clientes con riesgo de cancelación, logrando detectar una mayor proporción de casos positivos en comparación con la regresión logística.

---

## Conclusiones

- Los clientes con **menor tiempo de permanencia** presentan mayor probabilidad de cancelar el servicio.
- Los **contratos de corta duración** están más asociados con la cancelación.
- El modelo **Random Forest** logró capturar mejor los patrones del dataset para identificar clientes en riesgo de churn.

---

## Archivos del proyecto

- `TelecomX_LATAM_2.ipynb` → Notebook con todo el análisis y modelado.
- `TelecomX_Procesado.csv` → Dataset procesado utilizado para el entrenamiento de los modelos.
