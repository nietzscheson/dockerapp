FROM ubuntu:16.04

RUN apt-get update \ 
    && apt-get install -y nginx

RUN rm /etc/nginx/sites-enabled/default

ADD myapp.conf /etc/nginx/conf.d/myapp.conf
#ADD index.html /var/www/myapp/index.html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
