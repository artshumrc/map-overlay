FROM nginx:1.28-alpine

RUN apk add --no-cache apache2-utils

COPY nginx/default.conf /etc/nginx/conf.d/default.conf
COPY nginx/10-create-htpasswd.sh /docker-entrypoint.d/10-create-htpasswd.sh
RUN chmod +x /docker-entrypoint.d/10-create-htpasswd.sh