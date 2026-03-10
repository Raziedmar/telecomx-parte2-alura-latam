# 📊 Predicción de Cancelación de Clientes en TelecomX (Churn Prediction)

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Análisis%20de%20Datos-orange)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-yellow)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-red)

---

# 🚀 Descripción del Proyecto

La cancelación de clientes (**Churn**) es uno de los principales desafíos para las empresas de telecomunicaciones.
Cuando los clientes abandonan el servicio, la empresa pierde ingresos y debe invertir más recursos para adquirir nuevos clientes.

En este proyecto se desarrollan **modelos de Machine Learning capaces de predecir qué clientes tienen mayor probabilidad de cancelar su servicio** utilizando datos históricos de clientes de TelecomX.

El objetivo es **identificar clientes con alto riesgo de cancelación**, permitiendo a la empresa implementar estrategias de retención de manera anticipada.

---

# 🎯 Objetivos del Proyecto

* Preparar y transformar el dataset para el modelado predictivo.
* Realizar análisis exploratorio de datos (EDA).
* Entrenar modelos de clasificación para predecir churn.
* Evaluar el desempeño de los modelos mediante diferentes métricas.
* Identificar las variables que más influyen en la cancelación de clientes.
* Proponer recomendaciones estratégicas basadas en los resultados obtenidos.

---

# 📂 Dataset

El dataset contiene información de **7032 clientes** de TelecomX con variables relacionadas con sus servicios y facturación.

| Variable        | Descripción                                                 |
| --------------- | ----------------------------------------------------------- |
| Churn           | Indica si el cliente canceló el servicio                    |
| tenure          | Número de meses que el cliente ha permanecido en la empresa |
| Contract        | Tipo de contrato                                            |
| InternetService | Tipo de servicio de internet                                |
| PaymentMethod   | Método de pago                                              |
| Charges.Monthly | Cargo mensual                                               |
| Charges.Total   | Total pagado                                                |
| Cuentas_Diarias | Estimación del gasto diario                                 |

Este dataset corresponde al **dataset limpio generado en la Parte 1 del challenge TelecomX**.

---

# 🧹 Preparación de Datos

Durante el proceso de preparación se realizaron las siguientes tareas:

* Eliminación de columnas irrelevantes (`customerID`)
* Transformación de variables categóricas mediante **One-Hot Encoding**
* Verificación del desbalance de clases
* Normalización de variables utilizando **StandardScaler**
* División del dataset en **conjunto de entrenamiento y prueba (train/test)**

Estas transformaciones permiten que los datos estén listos para ser utilizados en modelos de Machine Learning.

---

# 📊 Análisis Exploratorio de Datos (EDA)

El análisis exploratorio permitió identificar patrones importantes relacionados con la cancelación de clientes.

Principales análisis realizados:

* Distribución de clientes que cancelan el servicio
* Análisis de correlación entre variables
* Relación entre **antigüedad del cliente (tenure) y churn**
* Relación entre **cargos mensuales y cancelación**

Estos análisis mostraron que algunas variables tienen una fuerte relación con la cancelación.

---

# 🤖 Modelos de Machine Learning

Se implementaron dos algoritmos de clasificación:

## 1️⃣ Regresión Logística

* Modelo de clasificación interpretable
* Permite entender la relación entre variables y churn

## 2️⃣ Random Forest

* Modelo de ensamblado basado en árboles de decisión
* Captura relaciones complejas entre variables
* Permite analizar la importancia de variables

Los modelos fueron entrenados con el conjunto de entrenamiento y evaluados con el conjunto de prueba.

---

# 📈 Evaluación de Modelos

Los modelos fueron evaluados utilizando las siguientes métricas:

* **Accuracy**
* **Precision**
* **Recall**
* **F1 Score**
* **Matriz de Confusión**

Estas métricas permiten medir qué tan bien los modelos identifican a los clientes que tienen mayor probabilidad de cancelar el servicio.

---

# 🔍 Importancia de Variables

Utilizando el modelo **Random Forest**, se identificaron las variables que más influyen en la predicción del churn.

Las variables más relevantes incluyen:

* **tenure (antigüedad del cliente)**
* **tipo de contrato**
* **cargos mensuales**
* **tipo de servicio de internet**
* **método de pago**

Estas variables explican gran parte del comportamiento de cancelación de los clientes.

---

# 💡 Principales Hallazgos

El análisis permitió identificar varios patrones importantes:

* Los clientes con **menor antigüedad presentan mayor probabilidad de cancelación**.
* Los clientes con **contratos mensuales tienen mayor tasa de churn**.
* Los **cargos mensuales elevados** pueden aumentar la probabilidad de abandono.
* El churn depende de múltiples factores combinados.

---

# 📊 Recomendaciones de Negocio

Basado en los resultados obtenidos, se sugieren las siguientes estrategias:

### Programas de retención temprana

Implementar estrategias de fidelización durante los primeros meses del cliente.

### Incentivar contratos de mayor duración

Ofrecer descuentos o beneficios para contratos anuales.

### Optimización de planes de precios

Revisar planes con cargos elevados que podrían generar mayor churn.

### Promoción de paquetes de servicios

Los clientes que contratan más servicios tienden a permanecer más tiempo.

Estas estrategias pueden ayudar a **reducir significativamente la cancelación de clientes**.

---

# 🛠 Tecnologías Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

# 📁 Estructura del Proyecto

```text
TelecomX-Churn-Prediction
│
├── TelecomX_LATAM_Parte2.ipynb
├── TelecomX_limpio.csv
├── README.md
```

---

# 👨‍💻 Autor

Proyecto desarrollado como parte del **Challenge TelecomX — Data Science LATAM**.

