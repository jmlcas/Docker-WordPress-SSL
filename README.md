# Docker-WordPress-SSL

Opcional:

Agregar estas líneas a "docker-compose" para ver la BBDD con Adminer

  adminer:
    container_name: adm
    image: adminer 
    restart: unless-stopped    
    depends_on:      
      - mysql
    ports:      
      - "8080:8080"        
    environment:
      MYSQL_ROOT_PASSWORD: ${MYSQL_ROOT_PASSWORD}
      ADMINER_USERNAME: ${MYSQL_USER}
      MYSQL_DATABASE: ${MYSQL_DATABASE}
      ADMINER_PASSWORD: ${MYSQL_PASSWORD}  
      
      
