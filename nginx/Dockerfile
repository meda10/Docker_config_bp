FROM nginx:latest

COPY conf.d/default.conf /etc/nginx/conf.d/default.conf
# COPY nginx.conf/nginx.conf /etc/nginx/nginx.conf

RUN apt-get update
RUN apt-get install openssl
COPY start.sh /start.sh
RUN chmod -R 777 /start.sh
CMD ["nginx", "-g", "daemon off;"]
CMD ["nginx", "-g", "daemon off;"]
ENTRYPOINT ["/bin/bash", "-c", "/start.sh"]