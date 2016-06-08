#Práctica 3

Esta práctica trata de la configuración de dos balanceadores de cargar ##nginx y ##haproxy. Para ellos necesitaremos los dos servidores configurados en prácticas anteriores
y un nuevo servidor que es donde se realizarán las modificaciones y las pruebas.

Primero mostraré la configuración de ##nginx.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica3/imagenes/configuracionnginx.png)

Ahora comprobamos que el servicio nginx esta activo, para ello el comando service nginx status.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica3/imagenes/nginx_status.png)

Por último, comprobaremos que está balanceando la carga con el mismo peso.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica3/imagenes/pruebanginx.png)

Ahora procedo a la configuración de ##haproxy

Primero muestro el archivo de configuración.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica3/imagenes/confhapr1.png)

y la parte final del archivo de configuración:

![imagen](https://github.com/marquirj/swap1516/blob/master/practica3/imagenes/confhapr2.png)

Lanzo el servicio de haproxy con el comando mostrado a continuación:

![imagen](https://github.com/marquirj/swap1516/blob/master/practica3/imagenes/lanzahapr.png)

Y ahora una prueba del funcionamiento de este balanceador.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica3/imagenes/haproxy.png)