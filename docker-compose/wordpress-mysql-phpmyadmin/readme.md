# Wordpress para desarrollo
Archivo de docker compose para desarrollo de plugins o themes de wordpress.

Este archivo crea los servicios de:
- Base de datos MySQL
- Core de wordpress
- PhpMyAdmin para la administración de la base de datos.

Para hacer posible el desarrollo, el core de wordpress se instala en una carpeta
local del host de nombre "wordpress" y que debe estar al mismo nivel que el archivo 
docker-compose.yml, esta carpeta se enlaza a la carpeta /var/www/html dentro
del contenedor.