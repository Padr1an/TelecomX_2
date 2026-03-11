# 📡 Proyecto Telecom X — Parte 2

Este repositorio contiene la fase de **Modelado Predictivo** y **Optimización** del proyecto Telecom X. Tras el análisis exploratorio inicial, este notebook se enfoca en la construcción de un sistema de alerta temprana para identificar clientes en riesgo de abandono.

## 🎯 Objetivo del Proyecto
Desarrollar un modelo robusto de clasificación que permita a **Telecom X** pasar de una cultura reactiva a una estrategia proactiva, reduciendo la tasa de deserción mediante la identificación automatizada de patrones de comportamiento.

## 🛠️ Stack Tecnológico
- **Lenguaje:** Python 3.x
- **Procesamiento:** Pandas, NumPy
- **ML & Modelado:** Scikit-Learn (Random Forest, GridSearchCV, Train-Test Split)
- **Evaluación:** Matrices de Confusión, R² Score, Classification Report
- **Visualización:** Matplotlib, Seaborn

## ⚙️ Metodología Aplicada
1. **Preprocesamiento Avanzado**: Limpieza final de datos y codificación de variables categóricas.
2. **Estrategia de Modelado**: Implementación de un **Random Forest Regressor/Classifier** para capturar relaciones no lineales entre las variables de consumo y la intención de fuga.
3. **Optimización de Hiperparámetros**: Uso de `GridSearchCV` para encontrar la configuración óptima de:
   - `max_depth` (Profundidad del árbol)
   - `n_estimators` (Cantidad de árboles en el bosque)
   - `min_samples_leaf` y `min_samples_split`
4. **Validación**: Aplicación de Validación Cruzada ($K$-Fold) para garantizar la estabilidad del modelo ante nuevos datos.

## 📊 Resultados y Métricas
- **Desempeño**: El modelo optimizado ofrece una alta capacidad de generalización, evitando el sobreajuste (*overfitting*).
- **Variables Críticas**: Se identificó que la antigüedad del cliente (`tenure`) y los cargos mensuales (`MonthlyCharges`) son los predictores con mayor peso en el modelo.

## 📋 Conclusiones de Negocio
Se entregan recomendaciones estratégicas basadas en el modelo, incluyendo:
- **Optimización de Pagos**: Incentivar el paso de "Electronic Check" a débitos automáticos.
- **Estrategia de Producto**: Auditoría de calidad sobre el servicio de Fibra Óptica.
- **Servicios Agregados**: Promoción de soporte técnico como barrera de salida.

## 🚀 Instrucciones de Ejecución
1. Asegúrese de tener las librerías instaladas:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
