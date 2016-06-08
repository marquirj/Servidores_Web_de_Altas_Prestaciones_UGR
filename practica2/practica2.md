#Práctica 2

En esta práctica consiste en sincronizar directorios entre dos servidores. Mi servidor 1 tiene la Ip: 192.168.1.100 y mi servidor 2 tiene la IP:192.168.1.101

#Parte rsync.

Primero hay que dar permiso a rootlogin en el directorio:  /etc/ssh/sshd_config

![imagen](https://github.com/marquirj/swap1516/blob/master/practica2/imagenes/rsync1.PNG)

Después compartimos un directorio.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica2/imagenes/rsync2.PNG)

#Parte ssh 

Una vez generada las clave la debemos copiar en el servidor 1 para ello se utiliza le siguiente comando.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica2/imagenes/ssh1.PNG)

Ahora comprobaremos que hemos podido tener acceso al servidor 1 desde el servidor 2.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica2/imagenes/ssh2.PNG)

#Parte crontab

Aqui simplemente mostraré el archivo que hay que editar con la última linea añadida que es la que queremos que se ejecute.

![imagen](https://github.com/marquirj/swap1516/blob/master/practica2/imagenes/crontab.ssh.PNG)

