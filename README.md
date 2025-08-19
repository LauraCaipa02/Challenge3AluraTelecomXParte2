# Challenge3AluraTelecomXParte2
Este es el challenge # 3 del programa ONE, la parte 2 del análisis de Churn para Telecom X


# Análisis de Cancelación de Clientes (Churn)

## Descripción del proyecto
Este proyecto tiene como objetivo analizar y predecir la **cancelación de clientes (churn)** en la empresa *Telecom X*.  
El análisis combina técnicas de exploración de datos y modelos de **machine learning**, con el fin de identificar los factores que influyen en la decisión de los clientes de abandonar el servicio y proponer estrategias efectivas de retención.

## Origen de los datos
Los datos fueron obtenidos desde el **Challenge Telecom X Parte 1**, disponible en GitHub.  
Se trabajó a partir de un archivo en formato **CSV** enlazado directamente desde el repositorio del reto.

## Metodología
1. **Recolección y preparación de datos**  
   - Importación del dataset desde GitHub en formato CSV.  
   - Proceso de limpieza, normalización y codificación de variables.  
   - Aplicación de **oversampling** para balancear las clases y evitar sesgos en el entrenamiento.  

2. **Exploración y análisis**  
   - Identificación de patrones de uso, cargos mensuales, tenencia y tipo de contrato.  
   - Análisis de servicios complementarios como seguridad en línea, soporte técnico e internet de fibra óptica.  

3. **Entrenamiento de modelos**  
   - Se entrenaron distintos modelos de clasificación (Regresión Logística, Random Forest, entre otros).  
   - Evaluación mediante las métricas de desempeño más relevantes:  
     - **Exactitud (Accuracy)**  
     - **Precisión (Precision)**  
     - **Recall (Sensibilidad)**  
     - **F1-score**  
     - **Matrices de confusión**, tanto en entrenamiento como en validación.  

4. **Control de overfitting y underfitting**  
   - Gracias a la técnica de **balanceo con oversampling**, se logró un modelo estable.  
   - No se observaron indicios de **overfitting ni underfitting**, ya que el desempeño se mantuvo consistente entre los conjuntos de entrenamiento y validación.  

## Resultados
- El modelo con mejor desempeño fue el **Random Forest con oversampling**, mostrando un equilibrio entre precisión y recall tanto en el conjunto de entrenamiento como en validación.  
- Entre las variables más influyentes en la cancelación se destacan:  
  - **Tenencia baja de clientes (tenure).**  
  - **Contrato mes a mes.**  
  - **Altos cargos mensuales y totales.**  
  - **Ausencia de servicios de seguridad en línea y soporte técnico.**  
  - **Clientes con internet de fibra óptica.**

## Estrategias de retención recomendadas
- Implementar **programas de fidelización temprana** para clientes con baja permanencia.  
- Incentivar la **migración de contratos mensuales a planes anuales o bianuales**.  
- Ofrecer **planes más flexibles y personalizados** para clientes con altos costos mensuales.  
- Potenciar la adopción de servicios complementarios como seguridad en línea y soporte técnico.  
- Revisar la **experiencia de clientes con fibra óptica** para reducir su tasa de salida.  

## Tecnologías utilizadas
- **Python 3.11**  
- **Pandas**, **NumPy** para manipulación y análisis de datos.  
- **Scikit-learn** para la construcción y evaluación de modelos.  
- **Imbalanced-learn** para técnicas de oversampling.  
- **Matplotlib** y **Seaborn** para visualización de resultados.  

## Estructura del proyecto
- `ChallengeTelecomX2.ipynb` → Notebook principal con todo el análisis, modelos y visualizaciones.  
- Dataset importado directamente desde el repositorio del **Challenge Telecom X Parte 1**.  

## Ejecución
1. Clonar este repositorio:  
   ```bash
   gh repo clone LauraCaipa02/Challenge3AluraTelecomXParte2
