FROM nginx

RUN apt-get update && apt-get install -y procps
COPY start.sh /
COPY nginx.conf /etc/nginx/
COPY nginx-secure.conf /etc/nginx/
COPY static /etc/nginx/static
COPY dhparams.pem /etc/ssl/private/
CMD /start.sh
