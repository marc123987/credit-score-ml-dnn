# Credit Score ML DNN

Este proyecto implementa un modelo de Red neuronal profunda (DNN) para la clasificación del dataset de German Credit Data y se compara su rendimiento respecto a una red más moderna ResNet.

## 📋 Descripción

El proyecto incluye:
- **Jupyter Notebook**: Notebook con el código en Python que implementa un modelo DNN simple y un modelo ResNet, ambos modelos entrenados con el dataset de German Credit Data y que posteriormente se compara su rendimiento

## 📋 Objetivo

Diseñar, entrenar y evaluar un modelo de red neuronal profunda para predecir la probabilidad de impago de clientes bancarios, utilizando un conjunto de datos realista.

## 🚀 Estructura del Proyecto

```
├── Implementación_DNN_y_ResNet.ipynb      # Jupyter Notebook
└── README.md          # Este archivo
```

## 📚 Tecnologías Utilizadas

- **Python 3.x**
- **scikit-learn**: Machine Learning
- **matplotlib**: Gráficas
- **numpy**: Computación numérica
- **pandas**: Manipulación de datos
- **tensorflow**: Implementación de redes neuronales
- **shap**: Interpretabilidad de modelos

## 📝 Notas

- El modelo fue entrenado con 80% del dataset completo de German Credit Data (800 muestras)
- Este proyecto es con fines educativos y demostrativos

## 📝 Reflexiones de lo aprendido

Es importante considerar múltiples métricas para evaluar un modelo, ya que por ejemplo solo utilizar el Accuracy puede ser engañoso para casos como el analizado en este proyecto, en donde las clases del dataset estaban desbalanceadas.

Aunque los modelos neuronales pueden resultar difícil de explicar, existen herramientas como SHAP que permite identificar las variables que tienen mayor impacto al momento de realizar predicciones, lo cual puede ser útil para detectar posibles sesgos que pueda estar realizando el modelo, o qué tanto de este sesgo se arrastra desde el dataset. Para esto, el análisis del dataset previo preprocesamiento es esencial para poder detectar si alguna dimensión está sobrerepresentada al revisar la distribución de sus datos.