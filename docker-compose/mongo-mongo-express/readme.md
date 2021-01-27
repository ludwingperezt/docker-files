# Mongo - mongo express
Ejemplo de archivo de docker-compose que pone en linea dos servicios:
- Una base de datos con mongodb
- Un servicio de administración web para el servicio de mongodb

El archivo docker-compose.yml depende de un archivo de inicialización de nombre
init-mongo.js el cual contiene un script en javascript para crear un usuario
con permisos de lectura y escritura en la base de datos de mongodb. Este archivo
debe estar al mismo nivel que el archivo docker-compose.yml