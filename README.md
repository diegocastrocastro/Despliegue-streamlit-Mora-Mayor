# Despliegue-streamlit-Mora-Mayor
En este proyecto se implementó un flujo completo de modelado predictivo con Python orientado a la detección de clientes que podrían entrar en mora mayor.

Construcción de modelos
-) Se entrenaron diferentes algoritmos de clasificación (ej. regresión logística, KNN, árboles de decisión, Random Forest). 
-) Se evaluaron con métricas de desempeño (precisión, recall, F1‑score, matriz de confusión) para determinar cuál ofrecía mejor capacidad de generalización.

Selección del modelo óptimo
-) El modelo con mejor rendimiento fue un Random Forest, gracias a su capacidad de manejar relaciones no lineales y variables heterogéneas. 
-) A pesar de que la base de datos presentaba un alto desbalance de clases (pocos casos positivos de mora frente a muchos negativos), se buscó el algoritmo que maximizara la detección de casos relevantes sin perder estabilidad en las métricas globales.

Despliegue de la solución
-) El modelo entrenado se serializó en un archivo .pkl para su reutilización en producción. 
-) Debido a que GitHub impone un límite de 25 MB y el archivo del modelo supera ese tamaño, se optó por almacenarlo en Google Drive y descargarlo dinámicamente en la aplicación. 
-) El despliegue se realizó mediante Streamlit, construyendo una interfaz interactiva que permite al usuario ingresar datos de clientes y obtener la predicción en tiempo real.

Aplicación práctica
-) La solución permite simular escenarios de riesgo crediticio y apoyar la toma de decisiones en gestión financiera. 
-) El enfoque refleja la importancia de combinar técnicas de machine learning con herramientas de despliegue accesibles para usuarios no técnicos.

RESUMEN

El desarrollo integra:

-) Python para el entrenamiento y evaluación de modelos. 
-) Random Forest como algoritmo seleccionado por su mejor desempeño. 
-) Manejo de desbalance de clases como reto central. 
-) Streamlit + Google Drive para el despliegue interactivo y la gestión de archivos grandes. 
-) En caso aplicado dentro del taller de la Maestría en Ciencia de Datos de la UPB, orientado a la predicción de mora mayor.
