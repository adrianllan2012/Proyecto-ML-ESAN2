# Proyecto Final: Predicción de Conversión y Optimización Bayesiana en Campañas Digitales

**Curso:** Machine Learning & Deep Learning — ESAN  
**Caso:** Inspirado en campañas digitales de telecomunicaciones (Datos Sintéticos)

---

## 📄 Descripción del Proyecto

Este proyecto implementa un pipeline end-to-end reproducible que:
1. Genera un dataset sintético de 50,000 interacciones de campañas digitales sin *data leakage*.
2. Ejecuta un **split temporal** (Train: Meses 1–8, Validation: Meses 9–10, Test: Meses 11–12).
3. Evalúa y compara modelos de Machine Learning (**Logistic Regression**, **Random Forest** y **XGBoost**).
4. Selecciona un modelo ganador mediante métricas balanceadas (`PR-AUC`, `AUC`, `F1-Score` y `Brier Loss`).
5. Implementa **Optimización Bayesiana (GP + UCB)** frente a **Random Search** para sugerir la mejor configuración prescriptiva de campaña.
6. Provee un **Simulador Ejecutivo** para evaluar combinaciones de negocio personalizadas.

---

## 📁 Estructura del Repositorio

* `Proyecto_Final_ML_Optimizacion_Bayesiana_ESAN.ipynb`: Notebook principal con la simulación, modelado y optimización.
* `README.md`: Documentación y guía de ejecución del proyecto.
* `requirements.txt`: Dependencias del entorno de Python.
* `dataset_sintetico.csv`: Dataset generado sintéticamente.
* `metricas_modelos.csv`: Resultados comparativos de los modelos en el conjunto de Test.
* `benchmark_bo_vs_random.csv`: Resultado del benchmark de 20 ejecuciones de BO vs Random Search.
* `recomendacion_bo.csv`: Configuración óptima de campaña recomendada por la capa prescriptiva.

---

## 🚀 Instrucciones de Ejecución

### Opción A: Google Colab (Recomendado)
1. Subir el archivo `Proyecto_Final_ML_Optimizacion_Bayesiana_ESAN.ipynb` a Google Colab.
2. Ir al menú superior: **Entorno de ejecución** -> **Ejecutar todas**.
3. Los archivos `.csv` de resultados se exportarán automáticamente en el entorno local.

### Opción B: Ejecución Local
1. Clonar el repositorio:
   ```bash
   git clone [https://github.com/adrianllan2012/Proyecto-ML-ESAN.git](https://github.com/adrianllan2012/Proyecto-ML-ESAN.git)
   cd Proyecto-ML-ESAN
