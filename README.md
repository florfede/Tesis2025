## 🎓 Predicción del Éxito de Nuevos Artistas en la Industria de la Música

Este repositorio contiene el código completo y los experimentos desarrollados en el marco de mi **Tesis de Maestría en Ciencia de Datos (2025)**, cuyo objetivo es **predecir las regalías futuras de artistas musicales emergentes** mediante el uso de **modelos de series temporales multivariadas**, **análisis de sentimiento con modelos de lenguaje** y **representación de relaciones mediante grafos**.

---

### 🧩 Descripción general
El proyecto integra datos económicos, sociales y textuales para modelar el **potencial de rentabilidad de los artistas** dentro de la industria musical contemporánea.  
Combina enfoques **estadísticos, de aprendizaje automático, de procesamiento del lenguaje natural (NLP)** y de **teoría de grafos** para construir pipelines predictivos capaces de capturar tanto patrones temporales como relaciones estructurales entre artistas.

---

### 🧠 Metodología
Los modelos implementados incluyen:

- **SARIMAX** → Modela dependencias temporales lineales con variables externas.  
- **Prophet** → Descompone tendencia y estacionalidad incorporando variables exógenas.  
- **XGBoost** → Algoritmo basado en boosting de árboles para regresión multivariada.  
- **LSTM (red neuronal)** → Captura dependencias de largo plazo en series secuenciales.  
- **RoBERTa (modelo de lenguaje)** → Realiza el **análisis de sentimiento** sobre textos de redes sociales, clasificando menciones positivas, negativas y neutras.  
- **Análisis de grafos** → Representa las **colaboraciones y conexiones entre artistas** para detectar comunidades, identificar nodos influyentes y explorar patrones de coautoría y difusión musical.

Cada **modelo de series temporales** (SARIMAX, Prophet, XGBoost y LSTM) se valida mediante esquemas de **walk-forward** o **ventana expansiva**, según su arquitectura.  
El desempeño de estos modelos se evalúa con las métricas **MSE**, **MAE**, **RMSE** y **MAPE**, tanto a nivel global como por artista.

---

### 📊 Datos
El dataset incluye **regalías mensuales de 15 artistas** durante un período de 3 a 4 años, enriquecidas con variables exógenas tales como:
- Seguidores en **Instagram** y **Twitter**  
- **Lanzamientos** de canciones  
- **Sentimiento** obtenido con **RoBERTa**, aplicado a comentarios y menciones en redes sociales  
- Métricas de **menciones e interacción**  
- **Relaciones de colaboración** entre artistas (grafos)

---

### ⚙️ Tecnologías utilizadas
Python • Pandas • NumPy • Scikit-learn • XGBoost • TensorFlow • Prophet • Statsmodels • Transformers (RoBERTa) • NetworkX • Matplotlib

---

### 📈 Resultados
Los resultados finales se consolidan en un **dashboard en Power BI**, que muestra las predicciones, las regalías históricas, la comparación de métricas entre modelos y la **visualización de redes de colaboración** entre artistas.  
El análisis de sentimiento complementa las proyecciones cuantitativas, permitiendo interpretar la **influencia emocional del público** sobre las variaciones en los ingresos.

---

### 📁 Estructura del repositorio
```text
├── datasets/            # Datasets preprocesados
├── notebooks/           # Desarrollo y evaluación de modelos (SARIMAX, Prophet, XGBoost, LSTM), análisis de sentimiento y grafos
├── results/             # Métricas y resultados consolidados para Power BI
└── README.md            # Descripción del proyecto (este archivo)
```

---

### ✍️ Autoría
**Autora:** Florencia Federico  
**Año:** 2025  
**Institución:** Maestría en Ciencia de Datos – Universidad Austral  
**Tutor:** Gustavo Denicolay  
