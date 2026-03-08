# Challenge-Telecom-X-Parte2

Propósito del análisis

Este proyecto tiene como objetivo desarrollar modelos predictivos capaces de identificar clientes con mayor riesgo de evasión (churn) en Telecom X. A partir de los datos tratados en la Parte 1 del desafío, se realiza una nueva etapa de preparación, análisis exploratorio y modelado con técnicas de machine learning para comprender qué variables influyen más en la cancelación del servicio.

El objetivo final es ayudar a la empresa a anticipar la pérdida de clientes y diseñar estrategias de retención basadas en datos.
---

Estructura del proyecto

El repositorio contiene los siguientes archivos:

TelecomX_Parte2.ipynb: notebook principal con el análisis, preparación de datos, modelado y conclusiones.
README.md: documentación general del proyecto.

---

Preparación de los datos

Para construir los modelos predictivos, se realizaron las siguientes etapas:

- Identificación de la variable objetivo (Churn) y separación de variables predictoras.
- Eliminación de registros con valores nulos en la variable objetivo.
- Clasificación de variables en categóricas y numéricas.
- Codificación de variables categóricas mediante One-Hot Encoding.
- Normalización o estandarización de variables numéricas cuando fue necesario, especialmente para modelos sensibles a escala como la Regresión Logística.
- Separación de los datos en conjuntos de entrenamiento y prueba.
- Evaluación del balance entre clases para interpretar correctamente las métricas del modelo.

Estas decisiones permitieron construir un pipeline de análisis adecuado para comparar distintos algoritmos de clasificación.

---

Análisis exploratorio e insights

Durante el análisis exploratorio se investigaron relaciones entre churn y variables relevantes como:
- antigüedad del cliente (tenure)
- cargo mensual (Charges.Monthly)
- tipo de contrato
- servicios contratados
- método de pago

Entre los hallazgos más relevantes, se observó que ciertos perfiles de clientes presentan mayor propensión a cancelar, especialmente aquellos con contratos de corto plazo y menor tiempo de permanencia en la empresa.

---

Modelos utilizados

Se entrenaron modelos de clasificación para predecir churn, incluyendo:

- Regresión Logística
- Random Forest

Los modelos fueron evaluados mediante métricas como:
- Accuracy
- Precision
- Recall
- F1-score
- ROC AUC

Además, se analizó la importancia de variables para interpretar qué factores tienen mayor impacto en la evasión de clientes.

---

Instrucciones de ejecución

1. Abrir el archivo TelecomX_Parte2.ipynb en Google Colab o Jupyter Notebook.
2. Asegurarse de que el archivo datos_tratados.csv esté en la misma ruta del notebook.
3. Instalar las bibliotecas necesarias si fuera necesario:

!pip install pandas numpy matplotlib seaborn scikit-learn

4. Ejecutar las celdas en orden para reproducir el análisis completo.

---

Tecnologías utilizadas
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

Conclusión

El análisis permitió identificar factores clave asociados a la cancelación de clientes en Telecom X. Variables como el tipo de contrato, la antigüedad del cliente y el cargo mensual mostraron una influencia significativa en la probabilidad de churn.
Entre los modelos probados, Random Forest mostró un mejor desempeño general en la predicción de churn, mientras que la Regresión Logística permitió una interpretación más clara del impacto de las variables.
Desde una perspectiva estratégica, Telecom X podría implementar acciones como:
- programas de fidelización para clientes nuevos,
- incentivos para contratos de mayor duración,
- monitoreo de clientes con alto cargo mensual,
- campañas de retención dirigidas a clientes con alta probabilidad de cancelación.

El uso de modelos predictivos permite a la empresa anticiparse a la pérdida de clientes y tomar decisiones basadas en datos, contribuyendo a mejorar la retención y la satisfacción del cliente.
cosas muy simples pero que en portafolios de Data Science se valoran mucho).
