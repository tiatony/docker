# Setup

Create your empty repository :
```
mkdir myrepo
```

Clone this repository :
```
cd myrepo
git clone git@github.com:tiatony/docker.git docker

```
launch Docker engine on your computer, then execute : 
```
cd docker
docker-compose up -d 
```

Create your Symfony project from the www container by executing : 
```
cd ../myrepo
docker exec www_kaamelott composer create-project symfony/website-skeleton project
```
(cf. https://symfony.com/doc/current/setup.html#creating-symfony-applications )

# Access 
- web server : http://localhost:8741
- Maildev : http://localhost:8081
- phpmyadmin : http://localhost:8080 (root / no password)
