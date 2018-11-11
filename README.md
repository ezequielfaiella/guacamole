# guacamole-docker-compose

#run
git clone https://github.com/gustonator/guacamole.git 
cd guacamole-docker-compose
cd init 
docker run --rm guacamole/guacamole:0.9.14 /opt/guacamole/bin/initdb.sh --postgres > initdb.sql
cd ..
docker-compose up -d

#To login, go to:
http://DOCKER_HOST:8080/guacamole/

user: 	  guacadmin
password: guacadmin
