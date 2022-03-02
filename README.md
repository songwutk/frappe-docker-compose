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

# Information

I'm new to docker. I can't create instant run frappe service, so please manual start by yourself.

# Size of my frappe image is  1.13GB


