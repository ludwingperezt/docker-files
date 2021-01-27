# Redis + RabbitMQ + PostgreSQL
Archivo de docker compose para utilizar la base de datos Redis, el gestor de 
colas RabbitMQ y una base de datos Postgres (generalmente se usa este stack
para aplicaciones desarrolladas con django).

Para el servicio de base de datos postgres se enlaza un directorio local
de nombre **db_backups** al directorio /root del contenedor, se hace esto para
tener acceso a archivos de backups a cargar al servidor o para generar archivos
de backups que deben estar disponibles fuera del servicio.  El directorio 
db_backups debe estar al mismo nivel que el archivo docker-compose.yml y no
es necesario que se llame db_backups.