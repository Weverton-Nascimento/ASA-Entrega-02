
FROM nginx:latest

COPY default.conf /etc/nginx/conf.d
COPY index.html /usr/share/nginx/html
COPY cert.crt /etc/nginx/ssl
COPY cert.key /etc/nginx/ssl

#RUN mkdir /etc/nginx/ssl
RUN chown -R root:root /etc/nginx/ssl
RUN chmod -R 600 /etc/nginx/ssl