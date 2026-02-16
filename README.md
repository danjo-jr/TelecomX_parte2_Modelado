# 📊 Telecom X – Predicción de Cancelación de Clientes (Churn)

## 📌 Descripción del Proyecto

Este proyecto forma parte del Challenge Telecom X del curso de Data Science.  
El objetivo fue desarrollar modelos de Machine Learning capaces de predecir qué clientes tienen mayor probabilidad de cancelar sus servicios (churn), además de identificar los factores que influyen en dicha decisión.

El trabajo abarca desde la limpieza y transformación de datos hasta la construcción, evaluación e interpretación de modelos predictivos.

---

## 🎯 Objetivo

Construir un modelo predictivo que permita anticipar la cancelación de clientes y extraer insights estratégicos que apoyen la toma de decisiones en estrategias de retención.

---

## 🧠 Modelos Implementados

Se entrenaron y evaluaron los siguientes modelos:

- 🔹 Regresión Logística (con normalización)
- 🔹 Random Forest
- 🔹 Random Forest con balanceo de clases

---

## 📊 Evaluación de Modelos

Las métricas utilizadas fueron:

- Accuracy
- Precision
- Recall
- F1-score
- Matriz de Confusión

### Resultados comparativos (conjunto de prueba)

| Modelo | Accuracy | Recall (Churn) | F1-score (Churn) |
|----------|------------|----------------|------------------|
| Regresión Logística | 0.79 | 0.27 | 0.41 |
| Random Forest | 0.79 | 0.43 | 0.53 |
| Random Forest (balanced) | 0.79 | 0.46 | 0.54 |

Aunque la exactitud fue similar en todos los modelos, Random Forest con balanceo de clases mostró mejor capacidad para detectar clientes que cancelan.

---

## ⚠️ Análisis de Overfitting y Underfitting

- La **Regresión Logística** mostró señales de underfitting, ya que su capacidad para detectar churn fue limitada (recall bajo).
- El **Random Forest** alcanzó 100% de accuracy en entrenamiento y ~79% en prueba, lo que evidencia overfitting.  
  Aun así, su desempeño en test fue estable y superior en detección de churn frente a los demás modelos.

---

## 🔍 Factores que Más Influyen en la Cancelación

El análisis de importancia de variables y coeficientes permitió identificar los principales factores asociados al churn:

### 🔴 Factores de mayor riesgo
- Baja antigüedad del cliente
- Contrato mensual
- Mayor cargo mensual
- Ausencia de servicios adicionales
- Menor número de servicios contratados

### 🟢 Factores de retención
- Mayor antigüedad
- Contratos anuales o bianuales
- Servicios como soporte técnico y seguridad en línea
- Mayor diversificación de servicios

---

## 💡 Recomendaciones Estratégicas

A partir de los resultados obtenidos, se proponen las siguientes acciones:

- Fortalecer la fidelización en los primeros meses del cliente.
- Incentivar la migración a contratos de mayor duración.
- Promover paquetes con servicios adicionales.
- Diseñar estrategias específicas para clientes con alto cargo mensual y contrato mensual.

---

## 🛠 Tecnologías Utilizadas

- Python  
- Pandas  
- NumPy  
- Scikit-Learn  
- Matplotlib  
- Seaborn  
- Google Colab  

---

## 📂 Estructura del Proyecto

- `TelecomX_LATAM.ipynb` → ETL y análisis exploratorio  
- `TelecomX_Parte2_Modelado.ipynb` → Modelado predictivo  
- `datos_tratados.csv` → Dataset procesado  

---

## 👤 Autor

Danilo José Álvarez Rodríguez  
Proyecto académico – Challenge Telecom X  
