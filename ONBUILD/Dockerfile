FROM almalinux:9
RUN dnf install nginx -y
RUN rm -f /usr/share/nginx/html/ondex.html
# This onbuild instruction runs only, when any user uses your image
ONBUILD COPY index.html /usr/share/nginx/html/ondex.html
CMD ["nginx", "-g", "daemon off;"]