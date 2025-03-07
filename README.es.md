# 📌 Aplicación de Técnicas de Extracción de Características en Clasificación de Imágenes  

### 📝 **Descripción**  
Este proyecto implementa un sistema de clasificación de imágenes basado en la extracción de características y aprendizaje automático. Se desarrollan y comparan dos algoritmos de extracción de características para analizar su efectividad en la clasificación de imágenes de animales en cuatro categorías: **gatos, elefantes, caballos y arañas**.  

Este proyecto fue desarrollado como trabajo final de la asignatura de Vision Artificial en tercer curso del grado de Ingeniería Informática en la Universidad Pública de Navarra (UPNA).

### 🎯 **Objetivos**  
✅ Implementar y evaluar dos algoritmos de extracción de características.  
✅ Aplicar diferentes modelos de aprendizaje automático para la clasificación.  
✅ Comparar los resultados obtenidos con cada enfoque.  

---

## 🔹 **Tecnologías Utilizadas**  
- **Python** 🐍  
- **scikit-learn** ⚙️ (Modelos de clasificación y validación cruzada)  
- **scikit-image** 🖼️ (Preprocesamiento de imágenes)  
- **NumPy & Pandas** 📊 (Manejo de datos)  

---

## 🔍 **Algoritmos de Extracción de Características**  

### 📌 **Algoritmo 1: Histogramas a partir de Transformación Binaria**  
- Convierte cada píxel en valores binarios comparando con sus vecinos.  
- Transforma los valores binarios a decimal y genera histogramas por bloques.  
- **Mejora:** Introducción de **transiciones uniformes** para reducir la complejidad.  

### 📌 **Algoritmo 2: Histogramas de Gradientes Orientados (HOG)**  
- Calcula la magnitud y orientación del gradiente en cada píxel.  
- Genera histogramas de 9 bins con la suma acumulada de magnitudes.  
- **Mejora:** **Normalización con bloques solapados** para mejorar la representación.  

---

## 📊 **Modelos Implementados**  

Se han probado distintos modelos de **aprendizaje automático**:  

- **SVM (Support Vector Machine)**  
- **Regresión Logística y Polinómica**  
- **Redes Neuronales (2 capas ocultas, 50 neuronas)**  
- **Técnicas de ensamblado:**  
  - **Bagging** (Bootstrap Aggregating)  
  - **Boosting (AdaBoost)**  
  - **Random Forest**  
- **Naive Bayes**  
- **Enfoques multiclase (OVO y OVA)**  

---

## 📈 **Resultados y Conclusiones**  

🔹 **Mejor modelo con el Algoritmo 1:** **Bagging**, con un rendimiento del **67.33% en validación cruzada** y **57.42% en prueba**.  

🔹 **Mejor modelo con el Algoritmo 2:** **Redes Neuronales**, con un rendimiento del **73.58% en validación cruzada** y **63.58% en prueba**.  

📌 **Conclusión:**  
El segundo algoritmo de extracción de características ha demostrado ser el más efectivo en este problema, obteniendo mejores resultados en la clasificación final.  
