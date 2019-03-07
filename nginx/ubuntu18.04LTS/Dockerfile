FROM ubuntu:18.04
RUN apt-get update && apt-get install -y \
       	git \
 	    vim \
        net-tools \
        nano
RUN apt-get install -y nginx	   
CMD ["nginx", "-g", "daemon off;"]