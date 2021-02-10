FROM nginx
ENV FLASK_SERVER_ADDR=flask:9091
COPY ./nginx.conf /tmp/nginx.conf
CMD [ "/bin/bash", "-c", "envsubst < /tmp/nginx.conf > /etc/nginx/conf.d/default.conf && nginx -g 'daemon off;'" ]