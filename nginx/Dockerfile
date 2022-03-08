FROM nginx:alpine

COPY ./nginx.conf /etc/nginx
RUN mkdir -p /etc/nginx/ssl
COPY ./elastic.crt /etc/nginx/ssl
COPY ./elastic.key /etc/nginx/ssl

WORKDIR /etc/nginx

CMD ["nginx", "-g", "daemon off;"]
