# docker-nginx-phalcon
docker phalcon nginx 

# start server
`
docker run  -p 80:80 -p 443:443 \
--name phalcon \
--link phalcon-mariadb:mysql \
-v /Users/river/PchomePay/cczone/deploy/:/var/www/ \
-v /Users/river/PchomePay/cczone/log:/var/log/nginx  \
-v /Users/river/PchomePay/cczone/log:/var/log/apache -d \
21e523e4a1f8
`