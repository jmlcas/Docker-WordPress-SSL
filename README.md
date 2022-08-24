# Docker-WordPress-SSL
WordPress + MySQL + phpMyAdmin + Nginx + SSL - CMS - Docker-compose

Ver en "localhost:80"

phpMyAdmin - ver en "localhost:8080"

Modificar las líneas 23 y 24 de docker-compose.yaml:

23  VIRTUAL_HOST: tudominio.com        #debe ser un dominio válido y DNS apuntando a este servidor
24  LETSENCRYPT_HOST: tudominio.com    #debe ser un dominio válido y DNS apuntando a este servidor   




