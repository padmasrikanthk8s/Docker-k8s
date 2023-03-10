FROM almalinux
LABEL AUTOR="PADMASRI" \
      COURSE="DOCKER"
ENV   ENV="PRD"
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
COPY evolve /usr/share/nginx/html/
ADD https://github.com/padmasrikanthk8s/Docker-k8s/blob/master/Docker/Dockerfile /tmp/
ADD terraform_1.4.0_linux_386.zip /tmp
EXPOSE 80
CMD ["nginx","-g","daemon off;"]