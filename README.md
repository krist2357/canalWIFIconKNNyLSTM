# ALTERNATIVAS PARA EL DISEÑO Y PLANIFICACIÓN DE REDES WIFI USANDO LOS ALGORITMOS KNN Y LSTM

El presente proyecto, intenta sugerir una idea para planificar y diseñar redes wifi en la banda de 2,4GHz.

Para esto, se ha tomado como base un dataset que contiene las siguientes características:

* SSID (nombre de la red)
* MAC address (Identificador del interface de radio)
* Vendor (Fabricante)
* Signal strength (Potencia de la señal en dBm)
* Channel (Identificador de frecuencia de la banda en uso).

La idea es identificar y cuantificar el nivel de interferencia en cada uno de los canales. Para esto se ha considerado cuantificar la cantidad de SSID presentes en un canal, por cada muestra tomada y también el nivel de señal presente en el canal dada por cada punto de acceso inalámbrico.

A continuación, se presentan los resulados para KNN:
![image](https://github.com/krist2357/canalWIFIconKNNyLSTM/assets/75154211/fc6ff3fc-e8b5-4a14-8252-80a261648923)

De forma similar para LSTM:
![image](https://github.com/krist2357/canalWIFIconKNNyLSTM/assets/75154211/3029347f-3d8d-46f7-a6bf-dc9528a453dc)

