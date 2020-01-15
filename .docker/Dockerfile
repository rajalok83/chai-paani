FROM php:7.0-apache
COPY . /srv/app
COPY .docker/vhost.conf /etc/apache2/sites-available/000-default.conf
RUN chown -R www-data:www-data /srv/app && a2enmod rewrite
#docker images -a | grep "none" | awk '{print $3}' | xargs docker rmi
#docker-machine stop
#docker-machine ls
#docker ps | grep "php" | awk '{print $1}' | xargs docker stop
#docker exec -it `docker ps | grep "php" | awk '{print $1}'` /bin/bash
#docker run --rm --network host -v $PWD/public:/srv/app/public:rw --name my-php php-app
#docker ps | grep "php" | awk '{print $1}' | xargs -r0 sh -c 'echo $1'
#docker ps | grep "php" | awk '{print $1}' | xargs -r0 sh -c 'echo $@'
#docker ps | grep "php" | awk '{print $1}' | xargs -r sh -c 'echo $@'
#docker ps | grep "php" | awk '{print $1}' | xargs sh -c 'echo $@'
#docker ps | grep "php" | awk '{print $1}' | xargs sh -c 'echo ${3}'