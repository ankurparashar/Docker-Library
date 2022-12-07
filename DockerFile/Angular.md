#### Angular DockerFile Template
```
FROM nginx

ARG BUILD="dev"

ENV BUILD=${BUILD}

## Set the permission for NGINX web folder
RUN chmod 777 -R /usr/share/nginx/html

## Overwrit the default NGINX config using the custom config file
COPY nginx.conf /etc/nginx/nginx.conf

## Remove default NGINX web files
RUN rm -rf /usr/share/nginx/html/*

COPY ./dist/<PROJECT>/ /usr/share/nginx/html

WORKDIR /usr/share/nginx/html

## Expose the docker port
EXPOSE 8080

## Initiate the NGINX
CMD ["nginx", "-g", "daemon off;"]
```
