FROM nginx:1-alpine

COPY ./etc /etc

RUN mkdir -p /var/run/nginx && chown -R nginx:nginx /var/cache/nginx /var/run/nginx /var/log/nginx

USER nginx
