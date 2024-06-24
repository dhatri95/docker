FROM almalinux:8
LABEL image="sleep" \
    Author="Dhatri"
#SEXPOSE 80/tcp 
# defaultly also it takes TCP only
ENV course="Devops" \
    topic=Docker
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
COPY index.html /usr/share/nginx/html/
CMD [ "nginx", "-g" , "daemon off;"]