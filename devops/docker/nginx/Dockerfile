FROM nginx:1.13.0-alpine

COPY default.conf /etc/nginx/conf.d

# Copy everything into the container, since we need the /vendor folder.
COPY ./webroot /usr/share/nginx