# Setup
Create the following directory structure into your project repository : 
|- docker
|- project

Go into docker repository and clone this repository :
```
cd docker
git clone git@github.com:tiatony/docker.git
```
launch Docker engine on your computer, then execute : 
```
docker-compose up -d 
```
it may take some time to process... 

Create your Symfony project from the www container by executing : 
```
cd ..
docker exec www_kaamelott composer create-project symfony/website-skeleton project
```

Access : 
- web server : http://localhost:8741
- Maildev : http://localhost:8081
- phpmyadmin : http://localhost:8080 (root / no password)
