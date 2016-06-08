#Práctica 6

En esta práctica crearemos un raid 1. Quitaremos un disco en caliente, simularemos un fallo y comprobamos que sigue funionando correctamente.

Primero realizo un fdisk -l para ver el estado del disco.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica6/imagenes/fdisk-l.PNG)

Montaremos el raid 1.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica6/imagenes/crearaid.PNG)

Una vez montado montariamos el sistema de archivos.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica6/imagenes/estado.PNG)

Ahora simularemos quitar un disco en caliente.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica6/imagenes/fallo.PNG)

Mostraré los detalles del raid.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica6/imagenes/detallefallo.PNG)

Quitaré un disco en caliente.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica6/imagenes/quitarcaliente.PNG)

Mostraré los detalles del raid de nuevo.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica6/imagenes/detallequitarcaliente.PNG)

Volveré a añadir el disco quitado anteriormente quitado.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica6/imagenes/anadir.PNG)

Y por últio mostraré de nuevo los detalles de que todo funciona correctamente.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica6/imagenes/detalleanadir.PNG)