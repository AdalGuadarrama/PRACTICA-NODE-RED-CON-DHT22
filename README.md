# PRACTICA-NODE-RED-CON-DHT22
En este repositorio se demuestra el método de programación del ESP32 con el sensor DHT11, además los datos obtenidos se reflejan en el programa Node-RED mediante una conexión WIFI.
## INTRODUCCION 
Usamos Esp32 en el ambiente de adquisición de datos, en esta práctica usaremos el sensor DTH11 para recolectar la temperatura y humedad del ambiente, también usaremos el programa Node-red para visualizar y programar esquemáticamente el flujo de información. Los resultados se pueden observar en la interfaz Node-Red, cabe señalar que en esta práctica se utilizará un simulador llamado WOKWI y un programa llamado Node-RED.
### MATERIAL 
Para la siguiente practica necesitaremos:
* programa WOKWI
* Programa Node-RED
* Tarjeta ESP 32
* Sensor DHT11
  #### INSTRUCCIONES
  Para poder realizar  esta practica  necesitaremos la ayuda la plataforma Node-red y WOKWI.
  1. Iniciamos sesion en nuestro Node-red y colocamos el bloque bloque mqqtt in.
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s0.0.png)
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s1.png)

   2. Configuramos el bloque con el puerto mqtt con el ip 18.193.219.109 y configuramos.
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s3%20(2).png)

   3. Colocamos un segundo  bloque con la descrioccion json y lo configuras como en la siguiente imagen.
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s4.png)

   4. Colocamos dos bloques function con el siguiente codigo, uno distinto para cada function.
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s5..png)
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s6.png)

   5. Colocamos los bloques Chart y Guage a cada una de las funciones y configuramos respectivamente.
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s7.png)
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s8.png)

    6. en la pestaña de de Layout crearemos otro tabulador llamado Sensor DHT22, dentro de el añadiremos dos grupos uno para los indicadores y otro para las graficas; de igual manera colocaremos dos espaciadores de temperatura y humedad, los pondremos segun sea el caso y la especificación.
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s9.png)

  7. Abrimos la terminal de programación WOKWI y colocar el iguiente codigo:
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s10.png)
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s11.png)

  8. Instalamos las librerias de DHT sensor library for ESPx, PubSubClient y ArduinoJson.
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s13.png)

  9. Para finalizar hacemos la conexion del sensor DHT11 con la ESP32.
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s12.png)

  10. colocamos la temperatura y humedad dando doble click al sensor DHT11 Iniciar, el simulador en Node-RED dando click izquierdo en el botón Deploy y despues abrir la interfaz.
![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s14.png)
  
  ##### RESULTADO
  * Visualizamos la interfaz y podremos manilular nuestro resltulados con el programa WOKWI.
  * Podras observar los valores dentro del monitor serial y la interfaz como se muestra.
  ![.](https://github.com/AdalGuadarrama/PRACTICA-NODE-RED-CON-DHT22/blob/main/s15.png)

  ##### CREDITOS
  Ing. Guadarrama Lome Adalberto.
