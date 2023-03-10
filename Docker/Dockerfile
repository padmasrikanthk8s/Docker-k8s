FROM almalinux
LABEL AUTHOR="padmasrikanth" \
      ENV="Prod" 
RUN yum install nginx -y
EXPOSE 80
CMD ["nginx","-g","daemon off;"]
