# Tarea 3
## Angel Piñero Andion

### La siguiente práctica es una lista de tareas que tenéis que hacer.

### Por cada tarea tenéis que ir poniendo los comandos utilizados y, brevemente, describir el proceso y como compruebas que se ha realizado lo pedido en un fichero (nombre "Readme.md") con formato markdown.

### Crear un repositorio en github para subir este fichero

### Cada dos apartados tenéis que hacer un commit nombrando el numero del apartado

### En la respuesta pon el enlace a tu repositorio en github

### Utiliza la imagen de Apache, tag 2.4 y apoyandote en la mini guía de docker sigue las instrucciones:

1. ### Descarga la imagen 'httpd' y comprueba que está en tu equipo.
    Descargamos la imagen de apache2 con el siguiente comando:
    ```docker pull httpd:2.4```
    Comprobamos que la imagen se ha descargado correctamente con el siguiente comando:
    ```docker images```
![apartado1.png](images/apartado1.png)

2. ### Crea un contenedor con el nombre 'dam_web1'.

    Creamos el contenedor con el siguiente comando:
    ```docker run -d --name dam_web1 httpd:2.4```
    Comprobamos que el contenedor se ha creado correctamente con el siguiente comando:
    ```docker ps```
![apartado2.png](images/apartado2.png)
3. ### Si quieres poder acceder desde el navegador de tu equipo, ¿que debes hacer?
4. ### Utiliza bind mount para que el directorio del apache2 'htdocs' esté montado un directorio que tu elijas.
5. ### Realiza un 'hola mundo' en html y comprueba que accedes desde el navegador.
6. ### Crea otro contenedor 'dam_web2' con el mismo bind mount y a otro puerto, por ejemplo 9080.
7. ### Comprueba que los dos servidores 'sirven' la misma página, es decir, cuando consultamos en el navegador:
    ### http://localhost:9080
    ### http://localhost:8000
8. ### Realiza modificaciones de la página y comprueba que los dos servidores 'sirven' la misma página