## 🎓 Predicción del Éxito de Nuevos Artistas en la Industria de la Música – Tesis de Maestría

Este repositorio contiene el código completo y los experimentos desarrollados en el marco de mi Tesis de Maestría en Ciencia de Datos, cuyo objetivo es predecir las regalías futuras de artistas musicales emergentes mediante el uso de modelos de series temporales multivariadas y análisis de sentimiento aplicado a redes sociales.

🧩 Descripción general

El proyecto integra datos económicos, sociales y textuales para modelar el potencial de rentabilidad de los artistas dentro de la industria musical contemporánea. Combina enfoques estadísticos y de aprendizaje automático para construir pipelines predictivos capaces de capturar tanto patrones temporales como efectos exógenos.

🧠 Metodología

Los modelos implementados incluyen:

- SARIMAX: para modelar dependencias temporales lineales con variables externas.
- Prophet: para descomponer tendencia y estacionalidad incorporando variables exógenas.
- XGBoost: basado en árboles de decisión y boosting para regresión multivariada.
- LSTM (red neuronal): para capturar dependencias de largo plazo en series secuenciales.

Cada modelo se valida mediante esquemas de walk-forward o ventana expansiva, según su arquitectura.
El desempeño se evalúa con métricas MSE, MAE, RMSE y MAPE, tanto a nivel global como por artista.

📊 Datos

El dataset incluye regalías mensuales de 15 artistas a lo largo de un período de 3 a 4 años, enriquecidas con variables exógenas tales como:
Seguidores en Instagram y Twitter
Lanzamientos de canciones
Sentimiento extraído de comentarios en redes sociales
Métricas de menciones e interacción


⚙️ Tecnologías utilizadas

Python • Pandas • NumPy • Scikit-learn • XGBoost • TensorFlow • Prophet • Statsmodels • Matplotlib

📈 Resultados

Los resultados finales se consolidan en un dashboard en Power BI, que muestra las predicciones, las regalías históricas y la comparación de métricas entre modelos para cada artista.

📁 Estructura del repositorio
```text
├── datasets/            # Datasets preprocesados
├── notebooks/           # Desarrollo y evaluación de modelos (SARIMAX, Prophet, XGBoost, LSTM), análisis de sentimiento y grafos
├── results/             # Métricas y resultados consolidados para Power BI
└── README.md            # Descripción del proyecto (este archivo)
