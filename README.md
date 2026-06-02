# Modelos_de_Clasificación
# 🎯 Estrategias de Clasificación y Optimización de Métricas de Negocio

Este repositorio contiene una serie de proyectos prácticos enfocados en la resolución de problemas de **Clasificación Supervisada**. El objetivo central no es solo entrenar modelos, sino aprender a ajustar el **umbral de decisión (threshold)** para alinear el rendimiento técnico con las necesidades financieras y operativas de diferentes sectores.

## 📂 Casos de Uso Implementados

### 1. Detección de Abandono Escolar (EdTech)
* **Objetivo:** Identificar alumnos en riesgo de desertar para intervención temprana.
* **Prioridad:** **Recall**. Minimizamos los Falsos Negativos (alumnos que se pierden sin ayuda).
* **Resultado:** Ajuste del threshold a **0.2**, logrando capturar al **96%** de los alumnos en riesgo.

### 2. Marketing de Lujo (Targeting de Precisión)
* **Objetivo:** Optimizar el envío de catálogos físicos de alto coste (80€/u).
* **Prioridad:** **Precision**. Aseguramos que cada envío tenga una probabilidad altísima de conversión.
* **Resultado:** Al subir el threshold a **0.8**, se redujo el desperdicio presupuestario en un **77%**, manteniendo una precisión superior al **92%**.

### 3. Mantenimiento Predictivo (Industria 4.0)
* **Objetivo:** Predecir fallos en maquinaria industrial con sensores de temperatura y vibración.
* **Estrategia:** Manejo de **datasets desbalanceados** (solo 10% de fallos) utilizando `RandomForestClassifier`.
* **Análisis de Coste:** Balanceo del impacto económico de un fallo no detectado (15.000€) frente a una revisión preventiva (500€).

## 🛠️ Stack Tecnológico
* **Modelos:** Logistic Regression, Random Forest, Decision Trees, KNN.
* **Evaluación:** Classification Report, Matrices de Confusión (falsos positivos vs. falsos negativos).
* **Optimización:** Manipulación de probabilidades (`predict_proba`) para el ajuste fino de métricas.

## 🧠 Aprendizajes Clave
1.  **El contexto define la métrica:** No existe el "mejor modelo" por defecto; la métrica reina depende de qué error es más costoso para el negocio.
2.  **Control del Umbral:** Capacidad para mover el punto de corte para intercambiar precisión por sensibilidad según la fase del proyecto.
3.  **Análisis de Costo-Beneficio:** Traducción de métricas estadísticas (F1-Score, Precision) a términos económicos (Euros ahorrados/ganados).

