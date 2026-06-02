# Modelos_de_Clasificación
# 🎯 Estrategias de Clasificación y Optimización de Métricas de Negocio

Este repositorio contiene una serie de proyectos prácticos de **Clasificación Supervisada** enfocados en la resolución de problemas críticos en entornos de producción real. El objetivo central es demostrar cómo el ajuste del **umbral de decisión (threshold)** alinea el rendimiento del modelo con las necesidades financieras y operativas de una organización.

## 📂 Casos de Uso e Impacto Económico

### 1. Detección de Abandono Escolar (EdTech)
* **Contexto Real:** Utilizado por plataformas como Coursera, Khan Academy o Duolingo.
* **Objetivo:** Identificar alumnos en riesgo de desertar basándose en su actividad académica.
* **Prioridad:** **Recall (Sensibilidad)**. El coste de "perder" a un alumno es mayor que el de enviar un mensaje de apoyo innecesario.
* **Resultado:** Ajuste del threshold a **0.1**, logrando capturar al **96.7%** de los alumnos en riesgo (solo 4 fallos no detectados).

### 2. Marketing de Lujo (Targeting de Precisión)
* **Contexto Real:** Estrategia habitual en marcas premium como Cartier, Loewe o Rolex.
* **Objetivo:** Optimizar el envío de catálogos impresos de alto coste (80€/unidad).
* **Prioridad:** **Precision**. Minimizar el desperdicio presupuestario ("Limpieza de basura").
* **Análisis del Threshold:** * Con umbral **0.5**: Se perdían 36 catálogos (2.880€ tirados a la basura).
    * Con umbral **0.8**: Solo se pierden 8 catálogos (640€).
    * **Impacto:** Ahorro directo de **2.240€** solo ajustando el parámetro a una precisión del **92.3%**. Se sacrifica alcance (Recall) por una inversión de alta rentabilidad.

### 3. Mantenimiento Predictivo (Industria 4.0)
* **Contexto Real:** Aplicado por gigantes industriales como GE, Siemens o Rolls-Royce.
* **Objetivo:** Predecir fallos críticos en maquinaria para evitar paradas de línea.
* **Análisis de Coste-Beneficio:** Un fallo no detectado cuesta **15.000€**, mientras que una revisión preventiva innecesaria cuesta **500€**.
* **Impacto del Ajuste Analítico:**
    * **Umbral 0.5 (Estándar):** 51 fallos no detectados. Pérdida operativa: **766.000€**.
    * **Umbral 0.1 (Optimizado):** Solo 4 fallos no detectados. 
    * **Resultado:** Reducción del coste total a **138.500€**. **Ahorro neto generado: 627.500€**.

## 🛠️ Stack Tecnológico
* **Modelos:** Logistic Regression, Random Forest, Decision Trees, KNN.
* **Librerías:** `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`.
* **Técnicas:** Manipulación de `predict_proba`, curvas de coste, manejo de datasets desbalanceados y optimización de umbrales.

## 🧠 Aprendizajes Clave
1.  **El contexto define la métrica:** No hay métrica "mejor" en abstracto; depende de qué error es más costoso para el negocio (15.000€ vs 500€).
2.  **El Threshold como Mando de Control:** Capacidad para intercambiar precisión por recall según la fase del ciclo de vida del producto.
3.  **Traducción Técnica a Euros:** Los modelos no solo arrojan porcentajes, sino que se traducen en ahorro financiero directo y eficiencia operativa.

