# 🌍 U-Net Multi-Segmentation Model on Satellite Imagery

Este proyecto fue desarrollado como parte de una prueba técnica para una posición de Data Scientist especializada en imágenes satelitales. 

## 🧠 Descripción

El objetivo fue construir un modelo de **segmentación semántica multiclase** utilizando una arquitectura **U-Net** para clasificar imágenes satelitales de alta resolución.

El dataset original incluía imágenes multibanda (RGB + NIR) junto con sus respectivas máscaras de segmentación en 5 clases de cobertura del suelo. Debido a que los datos no son públicos, no se incluyen en este repositorio.

## 🔍 Exploración de Datos (EDA)

En el análisis exploratorio:

- Se identificó que las imágenes estaban bien calibradas y sin valores nulos.
- Las bandas NIR se destacaron como clave para distinguir zonas con vegetación.
- Las máscaras segmentaban en 5 categorías: agua, vegetación, superficies impermeables, suelo desnudo y otras.

## 🛠️ Desarrollo del Modelo

- Se utilizó una arquitectura **U-Net** implementada con Keras.
- Preprocesamiento incluyó normalización, encoding de máscaras y manejo de datos multibanda.
- Se trabajó con métricas como **IoU** y **accuracy** para evaluar el desempeño.
- Se incorporó data augmentation para mejorar la generalización del modelo.

## 📈 Resultados

El modelo dio buenos resultados, se podría mejorar la cantidad de imágenes en cada batch y los epochs. 

## 👩‍💻 Tecnologías y Librerías Usadas

- Python
- TensorFlow / Keras
- NumPy, Matplotlib, Scikit-learn
- xarray (lectura y manipulación de archivos `netCDF`)

## 📬 Sobre mí

Este notebook fue desarrollado por **Maria Lara Rossetti**.  
Me interesa aplicar mis conocimientos en ciencia de datos a problemas reales con impacto ambiental y territorial.  
Podés encontrarme en [LinkedIn](https://www.linkedin.com/in/maria-lara-rossetti/).

---

> ⚠️ Nota: Este repositorio es únicamente para fines demostrativos.
