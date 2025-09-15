FROM nginx:1-alpine

COPY ./etc /etc

RUN mkdir -p /var/run/nginx && chown -R nginx:nginx /var/cache/nginx /var/run/nginx /var/log/nginx

USER nginx

HEALTHCHECK --interval=30s --timeout=3s --start-period=5s --retries=3 CMD curl --fail http://localhost/health || exit 1
