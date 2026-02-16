# 📊 Telecom X – Predicción de Cancelación de Clientes (Churn)

## 📌 Descripción del Proyecto

Este proyecto forma parte del Challenge Telecom X del curso de Data Science.  
El objetivo principal fue desarrollar modelos predictivos capaces de anticipar qué clientes tienen mayor probabilidad de cancelar sus servicios (churn), utilizando técnicas de Machine Learning.

El análisis incluye:

- Preparación y limpieza de datos
- Análisis exploratorio
- Balanceo de clases
- Entrenamiento y evaluación de modelos
- Interpretación de variables relevantes
- Propuestas estratégicas de retención

---

## 🎯 Objetivo

Construir un modelo predictivo que permita identificar clientes con alto riesgo de cancelación y analizar los factores que influyen en dicha decisión, con el fin de generar recomendaciones estratégicas para reducir el churn.

---

## 🧠 Modelos Implementados

Se entrenaron y compararon los siguientes modelos:

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

### Resultados principales

| Modelo | Accuracy | Recall (Churn) | F1-score (Churn) |
|----------|------------|----------------|------------------|
| Regresión Logística | 0.79 | 0.27 | 0.41 |
| Random Forest | 0.79 | 0.43 | 0.53 |
| Random Forest (balanced) | 0.79 | 0.46 | 0.54 |

🔎 Aunque la exactitud fue similar en todos los modelos, Random Forest con balanceo de clases mostró mejor desempeño en la detección de clientes que cancelan.

---

## 🔍 Principales Factores que Influyen en el Churn

El análisis de importancia de variables y coeficientes permitió identificar los siguientes factores clave:

### 🔴 Factores que aumentan la probabilidad de cancelación
- Contrato mensual
- Mayor cargo mensual
- Baja antigüedad
- Fibra óptica
- Facturación electrónica

### 🟢 Factores que reducen la probabilidad de cancelación
- Mayor antigüedad del cliente
- Contrato anual o bianual
- Servicios adicionales como soporte técnico y seguridad en línea
- Mayor número de servicios contratados

---

## 📈 Conclusiones

El churn está fuertemente asociado con la antigüedad y el tipo de contrato.  
Los clientes nuevos y con contratos mensuales presentan mayor riesgo de cancelación.

El modelo Random Forest balanceado permitió detectar aproximadamente el 46% de los clientes que cancelan, convirtiéndose en la mejor opción entre los modelos evaluados.

Este análisis no solo permite predecir cancelaciones, sino también entender qué variables influyen más en el comportamiento del cliente.

---

## 💡 Recomendaciones Estratégicas

A partir de los resultados obtenidos, se proponen las siguientes acciones:

- Implementar programas de fidelización durante los primeros meses del cliente.
- Incentivar la migración a contratos anuales.
- Promover la contratación de servicios adicionales (soporte técnico y seguridad).
- Diseñar estrategias diferenciadas para clientes con alto cargo mensual.

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

- `Challenge_TelecomX_LATAM.ipynb` → ETL y análisis exploratorio
- `Challenge_TelecomX_Parte2.ipynb` → Modelado predictivo
- `datos_tratados.csv` → Dataset limpio utilizado para el modelado

---

## 👤 Autor

Danilo José Álvarez Rodríguez  
Estudiante de Data Science  
Proyecto académico – Challenge Telecom X

---

## 🚀 Estado del Proyecto

✔ Finalizado  
✔ Modelos evaluados  
✔ Conclusiones estratégicas desarrolladas  
