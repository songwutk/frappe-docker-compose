# frappe-docker-compose

Manual start service

 docker-compose up -d
 
 docker exec -it frappe /bin/bash
 
 bench start

# create new site

docker exec -it frappe /bin/bash
rm sites/default.site -rf
bench new-site default.site --db-host mysql --mariadb-root-password rootdocker
bench use default.site
bench start
