FROM nginx:alpine3.18

COPY ./nginx/default.conf /etc/nginx/conf.d/default.conf
COPY ./nginx/ssl/chain.pem /etc/ssl/chain.pem
COPY ./nginx/ssl/fullchain.pem /etc/ssl/fullchain.pem
COPY ./nginx/ssl/privkey.pem /etc/ssl/privkey.pem