ARG VERSION
FROM almalinux:${VERSION}
LABEL AUTHOR="PADMASRI"
ENV ENV="DEV"
RUN yum install nginx -y
EXPOSE 80
WORKDIR /usr/share/nginx/html
COPY evolve .
ADD https://github.com/padmasrikanthk8s/Docker-k8s .
ENTRYPOINT ["nginx","-g","daemon off;"]
#USER nginx
#CMD ["nginx","-g","daemon off;"]
