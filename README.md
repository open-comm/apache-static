Static Apache Webserver Configuration
=====================================

Ready to use static apache2 web server docker-compose configuration 
for a traefik web proxy.

This configuration uses the official apache2 docker image:

* apache2 image on docker hub: https://hub.docker.com/_/httpd


Install
-------

```
# clone repository
git clone https://github.com/open-comm/apache-static.git

# move into directory
cd apache-static

# create www directory where your static web page files go
mkdir www

# copy and edit the sample environment file
cp sample.env .env

## open the .env file in a text editor and configure all
## values to your needs: DOMAIN, ROUTERNAME
```

Put all your html files into the `www` directory.


Usage
-----

```
# start apache web server
docker-compose up -d

# stop apache web server
docker-compose down

# upgrade container
docker-compose pull
```



