# Detección de anomalías en MTS con RL

Este repositorio contiene el código Python para un sistema de detección de anomalías en series temporales multivariadas (MTS) sintéticas, utilizando una combinación de un Autoencoder LSTM y un agente de Q-Learning.

## Descripción

El objetivo principal de este proyecto es desarrollar y evaluar un enfoque híbrido para la detección de anomalías en MTS.
Se entrena un **Autoencoder LSTM** para aprender los patrones de datos "normales" y generar una "puntuación de anomalía" (error de reconstrucción).
Posteriormente, un **agente de Q-Learning** es entrenado para clasificar estas MTS como normales o anómalas, basándose en características extraídas de las curvas de anomalía.
El sistema incluye un proceso de **Grid Search** para optimizar los hiperparámetros y esquemas de recompensa del agente de Q-Learning.

## Componentes

- [x] Generación de datos sintéticos
- [x] Autoencoder LSTM
- [x] Agente de Q-Learning base
- [x] Grid Search para el agente de Q-Learning
- [x] Evaluación y visualización

## Documentación

* Ver [informe.pdf](docs/informe.pdf)

## Cómo ejecutar el código

* La notebook `lstm_rl.ipynb` contiene toda la lógica para la generación de datos, el entrenamiento del autoencoder y el agente RL, la evaluación y la visualización
* Se puede abrir y ejecutar directamente en Google Colab accediendo al siguiente link: <https://colab.research.google.com/github/mmarando/rl1/blob/main/lstm_rl.ipynb>
