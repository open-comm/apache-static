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
git clone git@gitlab.wachter-jud.net:docker/apache-static.git

# move into directory
cd apache-static

# create www directory where your static web page files go
mkdir www

# copy and edit the sample configuration file
cp docker-compose.yml.sample docker-compose.yml
```

Edit docker-compose.yml and change the following value:

* `your.web.domain` the domain name under which this web server will be available

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



