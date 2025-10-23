FROM almalinux:9
RUN dnf install enginx -y
RUN rm -rf /usr/share/nginx/html/index.html
# this executes if any user uses your image as their base OS
ONBUILD COPY index.html /usr/share/nginx/html/index.html
CMD ["ENGINX", "g", "deamon off;"]

