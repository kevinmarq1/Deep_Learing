# Deep_Learning
Predicción de Engagement en Atracciones Turísticas mediante Deep Learning. Proyecto final del módulo de redes neuronales: incluye modelos híbridos basados en imágenes (CNN, ResNet18) y metadatos, análisis de resultados y comparativa entre arquitecturas simples y preentrenadas.
# 🧠 Predicción del Éxito de Atracciones Turísticas

Este proyecto aplica técnicas de Deep Learning para predecir si un punto de interés turístico generará un nivel de engagement **alto o bajo**, combinando información visual (imagen) y estructurada (metadatos).
---
## 🎯 Objetivo
Construir y comparar dos modelos:
1. **Modelo 1 (Propio)**: CNN y MLP diseñados desde cero.
2. **Modelo 2 (Multimodal con ResNet18)**: Utiliza una CNN preentrenada + MLP estructurado.
---
## 📁 Estructura del Repositorio
📦 proyecto-turismo/
│
├── Practica_final_DP.ipynb # Notebook con todo el análisis, modelos y resultados
├── requirements.txt # Dependencias exactas usadas
├── best_model.pt # Pesos del mejor modelo entrenado (Modelo 2)
├── memoria_tecnica.pdf # Documento explicativo completo del proyecto
├── README.md # Este archivo
---
## ⚙️ Requisitos

Se recomienda ejecutar el proyecto en **Google Colab** para aprovechar aceleración por GPU.

1. **Python 3.10+**
2. Instala los paquetes necesarios:

```pip install -r requirements.txt ```

🚀 Instrucciones de uso
Clona el repositorio:

bash
Copiar
Editar
git clone https://github.com/tu_usuario/proyecto-turismo.git
cd proyecto-turismo
Ejecuta el notebook en Google Colab:

Abre Practica_final_DP.ipynb en Google Colab.

Monta tu Google Drive cuando se te indique.

Asegúrate de tener la carpeta Proyecto en tu Google Drive con esta estructura:

css
Copiar
Editar
/Proyecto/
├── poi_dataset.csv
└── data_main/
    ├── poi_id_1/
    │   └── main.jpg
    ├── poi_id_2/
    │   └── main.jpg
    └── ...
Entrenamiento:

Si no existe un modelo entrenado, el notebook comenzará a entrenar automáticamente.

Puedes cargar un modelo preentrenado desde best_model.pt.

Evaluación:

Al finalizar, se evalúan ambos modelos en un conjunto de test y se comparan los resultados.

📊 Resultados
Modelo	Accuracy (Test)	Observaciones
Modelo 1 (Propio)	0.96	Mejor generalización, menor sobreajuste
Modelo 2 (ResNet18)	0.55	Arquitectura más compleja, peor desempeño

✨ Reflexiones
Este proyecto demuestra que un modelo bien ajustado y sencillo puede superar a uno más sofisticado si no se adapta correctamente. La clave estuvo en el preprocesamiento, arquitectura adecuada y validación constante.

📄 Créditos
Desarrollado por Kevin Márquez como práctica final del módulo de Redes Neuronales del bootcamp Big Data & Machine Learning de KeepCoding.

---
