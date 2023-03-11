ARG VERSION
FROM almalinux:${VERSION}
LABEL AUTHOR="PADMASRIKANTH" \
      COURSE="DOCKER"
ENV LANDSCAPE="TEST"
RUN yum install nginx -y
EXPOSE 80
WORKDIR /usr/share/nginx/html
COPY evolve .
ADD https://github.com/padmasrikanthk8s/Docker-k8s/blob/master/Docker/RREADME.md .
CMD ["nginx","-g","daemon off;"]
