# PT2_Alura_TelecomX_Challenge
📝 Resumen del Proyecto
Este proyecto de ciencia de datos se enfoca en la predicción de la cancelación del servicio (Churn) de clientes para la empresa de telecomunicaciones TelecomX. El objetivo principal es identificar los factores que más influyen en que un cliente decida irse y, a partir de ello, construir un modelo de machine learning que pueda predecir con precisión cuáles clientes tienen mayor riesgo de abandono.

<br>

🛠️ Tecnologías y Librerías Utilizadas
Python: El lenguaje de programación principal del proyecto.

Pandas: Para la manipulación y análisis de datos.

NumPy: Para operaciones numéricas eficientes.

Scikit-learn: Para la creación, entrenamiento y evaluación de los modelos de machine learning.

Matplotlib y Seaborn: Para la visualización de datos y la exploración (EDA).

<br>

📊 Conjunto de Datos
El análisis se basa en el archivo datos_tratados.csv, que contiene información detallada sobre los clientes de TelecomX, creado en la primera parte de este proyecto, incluyendo:

Datos del cliente: Género, edad, si tienen pareja o dependientes.

Servicios: Tipo de servicio de internet (DSL, fibra óptica), múltiples líneas telefónicas, servicios adicionales como seguridad en línea, etc.

Información de la cuenta: Antigüedad del cliente, tipo de contrato, facturación mensual y total, y método de pago.

<br>

🤖 Modelos de Machine Learning y Resultados
Se implementaron y evaluaron varios modelos de clasificación para determinar cuál ofrecía el mejor rendimiento en la predicción del Churn.

Modelo	 Accuracy	Precision	Recall	F1-Score	ROC AUC Score
Naive Bayes Gaussiano	76.0%	55.0%	57.0%	56.0%	81.0%
Regresión Logística	80.0%	65.0%	53.0%	58.0%	81.0%
Random Forest	79.0%	63.0%	48.0%	54.0%	79.0%
SVC (SVM)	77.0%	57.0%	53.0%	55.0%	79.0%
K-Vecinos más Cercanos	76.0%	53.0%	57.0%	55.0%	75.0%

Exportar a Hojas de cálculo
Los modelos con el mejor desempeño, según la métrica ROC AUC Score, fueron el Naive Bayes Gaussiano y la Regresión Logística. Esta métrica es especialmente útil en este proyecto, ya que el conjunto de datos de Churn suele estar desequilibrado.

<br>

🔑 Factores Clave del Churn
El análisis de los modelos identificó las siguientes variables como las más importantes para predecir la cancelación del servicio:

Tipo de Contrato: Los clientes con contratos mes a mes son más propensos a irse.

Antigüedad del Cliente (Tenure): A menor antigüedad, mayor es el riesgo de churn.

Servicio de Internet: El servicio de fibra óptica se correlaciona con una mayor tasa de churn.

Método de Pago: Los clientes que usan cheque electrónico tienen un mayor riesgo de abandono.

<br>

💡 Conclusiones y Recomendaciones
El proyecto logró construir modelos de clasificación efectivos que pueden ser utilizados para predecir el churn. Las conclusiones extraídas del análisis de las variables más importantes ofrecen a TelecomX una guía clara para tomar decisiones estratégicas. Para reducir la tasa de abandono, la empresa podría:

Implementar programas de retención dirigidos a los clientes nuevos y aquellos con contratos mensuales.

Investigar y solucionar las posibles deficiencias del servicio de fibra óptica.

Estudiar la experiencia de los clientes que utilizan el cheque electrónico como método de pago.
