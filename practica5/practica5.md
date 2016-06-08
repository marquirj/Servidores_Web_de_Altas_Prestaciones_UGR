#Práctica 5

En esta práctica vamos a mostrar una base de datos creada y realizaremos una copia con mysqldump , después restauraremos esa copia de seguridad en otra máquina con mysql,  y replicaremos
máquinas con la configuración maestro-esclavo.

Lo primero que haré será enseñar la base de datos creada.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica5/imagenes/muestrabd.png)

Lo próximo que haremos será sera ejecutar el siguiente comando: mysqldump ejemplodb -u root -p > /root/ejemplodb.sql

![imagen](https://github.com/marquirj/swap1516/blob/master/practica5/imagenes/mysqldump.png)
Comprobamos con un ls que se ha creado un archivo .sql.

Ahora vamos a copiar con orden scp este archivo creado anteriormente en la segunda máquina.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica5/imagenes/copiarmaquina2.png)

Por último de este punto restauraremos la copia en la segunda máquina.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica5/imagenes/restaurarcopiamaquina2.png)

#Maestro-esclavo.

Mostraré el archivo de configuración de mysql.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica5/imagenes/confmysq.png)

Ahora crearemos un usuario que le daremos los siguientes permisos.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica5/imagenes/usuario.png)

Ahora se mostraría el estado del master ya que vamos a irnos en el siguiente paso al esclavo.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica5/imagenes/masterstatus.pnh.PNG)

Cambiamos los privilegios del master de la siguiente formas.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica5/imagenes/changemaster.PNG)

Arrancamos el esclavo con el comando start slave dentro de mysql.

Y mostramos el estado del esclavo con el siguiente comando.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica5/imagenes/replica.PNG)

