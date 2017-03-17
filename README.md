# LaraD-SQLSrv
Dockerfile config to create a Docker image based on Debian Jassie ready to deploy a Laravel App and connect to Microsoft Sql Server 2008/2012

Build And Run container on Widows as follow:

docker build -f Dockerfile-PHP56 -t LaraD-SQLsrv:dev .
docker run -v //c/Development/app:/var/www -v //c/Development/apache/000-default.conf:/etc/apache2/sites-available/000-default.conf  -p 80:80 LaraD-SQLsrv:dev

Build And Run container on Lunux/Mac as follow:

docker build -f Dockerfile-PHP56 -t LaraD-SQLsrv:dev .
docker run -v Development/app:/var/www -v Development/apache/000-default.conf:/etc/apache2/sites-available/000-default.conf  -p 80:80 LaraD-SQLsrv:dev

Point your browser to http://localhost

*CORS enabled in Apache
