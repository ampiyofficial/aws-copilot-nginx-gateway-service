FROM nginx:alpine
RUN rm /etc/nginx/conf.d/*.conf
COPY conf.d/*.conf /etc/nginx/conf.d/
CMD nginx -g "daemon off;"
EXPOSE 80
COPY ./favicon.png /usr/share/nginx/html/favicon.png
COPY ./index.html /usr/share/nginx/html/index.html

