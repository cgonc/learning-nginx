FROM ubuntu:18.04
RUN apt-get update && apt-get install -y \
        nginx \
       	git \
 	    vim \
        net-tools \
        nano \
        unzip
RUN  mkdir -p /sites/demo
ADD site/demo-site.zip /sites/demo
WORKDIR /sites/demo
RUN unzip demo-site.zip -d /sites/demo

COPY conf/nginx.conf /etc/nginx
CMD ["nginx", "-g", "daemon off;"]