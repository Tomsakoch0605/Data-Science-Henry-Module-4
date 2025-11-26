📊 FinanceGuard - Predicción de Churn Bancario

Sistema predictivo de abandono de clientes para banca digital utilizando Machine Learning y técnicas de análisis avanzado.

🎯 Descripción del Proyecto
FinanceGuard es un banco digital que enfrenta una tasa anual de abandono de clientes del 20%. Este proyecto desarrolla un sistema completo de predicción de churn que combina modelos supervisados, técnicas de ensamble y análisis no supervisado para identificar clientes en riesgo y facilitar estrategias de retención efectivas.
El proyecto analiza datos de 50,000 clientes incluyendo:

Variables demográficas (edad, género, ubicación, antigüedad)
Variables financieras (saldo promedio, productos contratados, transacciones)
Variable objetivo: churn (1 = abandonó, 0 = activo)

📂 Estructura del Proyecto

├── 1_EDA_RegresionLogistica.ipynb          # Análisis exploratorio y modelo baseline

├── 2_GradientBoosting_Optimizacion.ipynb   # Modelos avanzados y ensambles

├── 3_AprendizajeNoSupervisado.ipynb        # Clustering y reducción dimensional

└── README.md

🔍 Componentes del Proyecto

1️⃣ Análisis Exploratorio y Regresión Logística
Notebook: 1_EDA_RegresionLogistica.ipynb

EDA completo del dataset de clientes bancarios
Preprocesamiento de datos:

Tratamiento de valores faltantes
Encoding de variables categóricas
Escalamiento de variables numéricas
Análisis de multicolinealidad


Regresión Logística como modelo baseline:

Implementación con scikit-learn
Interpretación de coeficientes y odds ratios
Evaluación con matriz de confusión, ROC-AUC, Precision, Recall, F1-Score



2️⃣ Gradient Boosting y Optimización
Notebook: 2_GradientBoosting_Optimizacion.ipynb

Modelos de Gradient Boosting:

Random Forest
XGBoost (con optimización de hiperparámetros vía Grid Search)
LightGBM
CatBoost


Técnicas de validación:

StratifiedKFold para datos desbalanceados
Métricas especializadas (ROC-AUC, PR-AUC)


Ensamble de modelos:

Stacking con meta-learner (Regresión Logística)
Comparación de performance entre modelos



3️⃣ Aprendizaje No Supervisado
Notebook: 3_AprendizajeNoSupervisado.ipynb

Clustering de clientes:

K-Means (método del codo, coeficiente de silueta)
DBSCAN (detección de outliers)


Reducción de dimensionalidad:

PCA (análisis de componentes principales)
t-SNE (visualización no lineal)


Segmentación aplicada:

Identificación de 3-5 segmentos principales
Análisis de tasa de churn por segmento
Perfiles de clientes por cluster



🛠️ Stack Tecnológico

Python 3.8+
Análisis de datos: Pandas, NumPy
Machine Learning: Scikit-learn, XGBoost, LightGBM, CatBoost
Visualización: Matplotlib, Seaborn
Optimización: Optuna (opcional)
Entorno: Jupyter Notebooks / Google Colab

📊 Resultados Clave
El proyecto implementa una metodología completa desde el modelo baseline hasta técnicas avanzadas de ensamble, permitiendo:

✅ Identificación de clientes con alta probabilidad de abandono
✅ Comprensión de factores que influyen en el churn
✅ Segmentación de clientes por comportamiento
✅ Comparación rigurosa de múltiples algoritmos de ML
✅ Optimización de hiperparámetros para máximo rendimiento

🚀 Cómo Usar

Instalar dependencias:

bashpip install pandas numpy scikit-learn xgboost lightgbm catboost matplotlib seaborn
```

3. **Ejecutar notebooks en orden:**
   - Primero: `1_EDA_RegresionLogistica.ipynb`
   - Segundo: `2_GradientBoosting_Optimizacion.ipynb`
   - Tercero: `3_AprendizajeNoSupervisado.ipynb`

## 📈 Metodología

1. **Baseline Model:** Regresión Logística para establecer referencia
2. **Advanced Models:** Gradient Boosting con optimización de hiperparámetros
3. **Ensemble Learning:** Stacking para mejorar predicciones
4. **Unsupervised Learning:** Clustering para descubrir patrones ocultos
5. **Feature Engineering:** Creación de features derivadas del clustering

## 🎓 Aprendizajes

- Implementación completa de pipeline de ML para clasificación
- Manejo de datos desbalanceados en problemas de churn
- Optimización de hiperparámetros con Grid Search
- Técnicas de ensamble (Stacking)
- Análisis no supervisado complementario
- Interpretabilidad de modelos

## 📝 Licencia

Este proyecto fue desarrollado como parte del Proyecto Integrador 4 del programa de Ciencia de Datos.

## 👤 Autor
Michel Alejandro Carrillo Vázquez
Científico de Datos Junior
