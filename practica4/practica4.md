#Práctica 4

Esta práctica consiste en la medición de tiempo con los benchmarks de apache.

Para ellos utilizaremos una máquina con apache sirviendo una página web, y desde el terminal de otra máquina en la misma red
ejecutaremos el siguiente comando: 

ab -n 1000 -c 5 http://192.168.1.101/index.html

Mostraré una tabla con 10 ejecuciones del comando anterior.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica4/imagenes/tabla1.PNG)

Ahora dos gráficas correspondientes a: 

#Time taken per request

![imagen](https://github.com/marquirj/swap1516/blob/master/practica4/imagenes/col1.PNG)

#Request per seconds

![imagen](https://github.com/marquirj/swap1516/blob/master/practica4/imagenes/rqpersec1.PNG)

No muestro el campo de fallos ya que no han surgido fallos y las columna simpre obtiene el valor 0.

#Benchmark en nginx

Ahora ejecutaremos el mismo comando pero mandandolo a la dirección de nuestro balanceador de carga.

Tabla correspondiente a 10 ejecuciones.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica4/imagenes/tabalblanceador.PNG)

Lo siguente es mostrar una gráfica con:

#Time taken per request
![imagen](https://github.com/marquirj/swap1516/blob/master/practica4/imagenes/nginx1.PNG)
#Request per seconds
![imagen](https://github.com/marquirj/swap1516/blob/master/practica4/imagenes/nginx3.PNG)
#Benchmark en haproxy
 Ahora mostraré la tabla de diez ejecuciones con haproxy
![imagen](https://github.com/marquirj/swap1516/blob/master/practica4/imagenes/haproxytabla.PNG)
#Request per seconds
![imagen](https://github.com/marquirj/swap1516/blob/master/practica4/imagenes/haproxy3.PNG)
#Time taken per request
![imagen](https://github.com/marquirj/swap1516/blob/master/practica4/imagenes/haproxy11.PNG)
