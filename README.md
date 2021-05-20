# Training - HTML desafio

Objetivo mostrar el siguiente resultado en un HTML:

![image](https://user-images.githubusercontent.com/84411324/119030242-9f500380-b977-11eb-885c-d218db192965.png)

#Creando el la imagen partiendo del archivo Dockerfile#

sudo docker buil -t miapache /home/labjona/miweb

#Donde "miapache" es el nombre de la imagen seguido "/home/labjona/miweb" referente a la ubicacion donde se encuentra el archivo Dockerfile#

#Siguiente comando para correr nuestro contenedor# 

sudo docker run -d -p 80:80 --name webjona -v /home/labjona/miweb/:/var/www/html/ miapache

#Donde "webjona" es el nombre asociado al contenedor, "/home/labjona/miweb/" ruta de donde copiaremos los archivos about.html y index.html destino "/var/www/html/" seguido del nombre de imagen "miapache"#
