# 🛰️ Optimización de Espectro WiFi mediante KNN y LSTM

Este repositorio representa mi **primer proyecto de integración tecnológica**, desarrollado como parte de mi formación en la **Maestría en Inteligencia Artificial (UNIR)**. El objetivo es resolver un problema crítico en telecomunicaciones: la planificación eficiente de canales en la banda de 2.4 GHz mediante modelos predictivos.

## 📝 El Desafío de Ingeniería
En entornos densos, la interferencia co-canal y de canal adyacente degrada significativamente la calidad del servicio (Denominado QoS). En este sentido,, identifiqué la necesidad de pasar de una planificación estática a una **Gestión dinámica basada en datos**.

La idea es identificar y cuantificar el nivel de interferencia en cada uno de los canales. Para esto se ha considerado cuantificar la cantidad de SSID presentes en un canal, por cada muestra tomada y también el nivel de señal presente en el canal dada por cada punto de acceso inalámbrico.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python (Pandas, NumPy).
* **Deep Learning:** TensorFlow / Keras (Arquitectura LSTM).
* **Machine Learning:** Scikit-Learn (Algoritmo KNN).
* **Procesamiento:** StandardScaler para normalización de señales (dBm).
* **Entorno:** Google Colab / Jupyter Notebook.

## 🧠 Metodología: Comparativa de Modelos
El proyecto evalúa dos enfoques distintos para la toma de decisiones:
1. **K-Nearest Neighbors (KNN):** Implementado para clasificar niveles de interferencia basados en la densidad de SSIDs y potencia de señal.
2. **Long Short-Term Memory (LSTM):** Una red neuronal recurrente diseñada para capturar la naturaleza temporal de las señales inalámbricas, permitiendo predecir comportamientos futuros del espectro.

## 📈 Conclusiones Técnicas
* **Captura de Dependencias:** El modelo LSTM demostró una capacidad superior para entender que la interferencia de red no es un evento aislado, sino una serie temporal con tendencias.
* **Optimización Operativa:** La integración de estos modelos permite reducir el solapamiento de canales, mejorando la eficiencia operativa en el despliegue de infraestructuras Wi-Fi.
* **Escalabilidad:** Este enfoque sienta las bases para sistemas aplicados a redes WLAN empresariales.

## 📂 Estructura del Proyecto
* `Estudio_canal_wifi_1.ipynb`: Notebook con el análisis exploratorio (EDA), entrenamiento y evaluación de modelos.
* `wifi_data.csv`: Dataset con métricas reales de SSID, MAC Address, Vendor y Signal Strength.

## 📊 Resultados y Visualizaciones

El análisis comparativo arrojó métricas clave que validan el uso de arquitecturas recurrentes para este problema físico:



### Rendimiento del Modelo LSTM
* **Error Cuadrático Medio (MSE):** Se logró una reducción constante de la pérdida durante las 100 épocas de entrenamiento, estabilizándose en valores óptimos que indican una alta capacidad predictiva de la potencia de señal (RSSI).
* **Capacidad de Predicción:** A diferencia de KNN, la red LSTM logró seguir la tendencia de atenuación y ruido en el tiempo, lo que permite anticipar zonas de sombra en la cobertura WiFi.

### Comparativa Visual
El proyecto genera visualizaciones críticas para la toma de decisiones:
1. **Histogramas de Potencia:** Distribución de señales por fabricante (Vendor) para identificar saturación.
2. **Curva de Aprendizaje:** Gráfico de *Loss vs Epochs* que demuestra la convergencia del modelo de Deep Learning.
3. **Mapas de Interferencia:** Identificación de canales críticos en la banda de 2.4 GHz.

### Visualización de Resultados

| Clasificación por Canales (KNN) | Convergencia del Modelo (LSTM) |
| :---: | :---: |
| <img src="./KNN.png" width="400"> | <img src="./LSTM.png" width="400"> |

---
**Perfil del Autor:**
Soy **Christian Cadena**, Especializado en Electrónica, Telecomunicaciones e IA. Este proyecto marca el inicio de mi trayectoria integrando el desarrollo de software (Python) y la Inteligencia Artificial en el sector de la infraestructura tecnológica.
