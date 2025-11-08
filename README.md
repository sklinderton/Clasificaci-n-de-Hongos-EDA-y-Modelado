# Clasificación de Hongos (Mushrooms) — EDA + Modelado

**Fuente del dataset:** `mushrooms.csv` (clase objetivo: `class`, valores: `e=edible`, `p=poisonous`).  
**Paquete EDA del profesor:** `PaqEda.py` (clase `analisisEDA`).

## Objetivos
1. Aplicar un **EDA completo** del dataset.
2. Implementar **múltiples modelos** con **varios algoritmos** (≥5 algoritmos y ≥5 modelos).
3. Evaluar cada modelo con **indicadores vistos en clase**: *accuracy*, *error*, *precision/recall/F1 por clase*, *AUC* (cuando aplicable) y **matriz de confusión**.
4. Elaborar un **cuadro comparativo** y **gráficas** (distribución de clase, cardinalidad por atributo, **mapa de calor de correlaciones** sobre variables one-hot, importancia de variables, barras comparativas de métricas).

## Atributos (resumen)
- **class** *(objetivo)*: `e`=edible, `p`=poisonous  
- Otras columnas categóricas: `cap-shape`, `cap-surface`, `cap-color`, `bruises`, `odor`, `gill-attachment`, `gill-spacing`, `gill-size`, `gill-color`, `stalk-shape`, `stalk-root`, `stalk-surface-above-ring`, `stalk-surface-below-ring`, `stalk-color-above-ring`, `stalk-color-below-ring`, `veil-type`, `veil-color`, `ring-number`, `ring-type`, `spore-print-color`, `population`, `habitat`.

## Metodología
- Limpieza básica: duplicados, tipos, valores faltantes.
- Codificación **One-Hot** de todas las categóricas.
- Partición **estratificada** de *train/test* (80/20).
- **Modelos** evaluados (ejemplos): *Logistic Regression*, *Linear SVM*, *KNN*, *Decision Tree*, *Random Forest*, *Gradient Boosting*, *BernoulliNB*.
- Selección del **mejor** por *accuracy* (y AUC si aplica) y análisis de errores.

## Entregables
- Notebook ejecutable: **`Clasificacion_Mushrooms_EDA_Modelado.ipynb`**
- Resultados en tabla y gráficos dentro del notebook.
