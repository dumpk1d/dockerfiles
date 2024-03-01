#-----------------------------------------------------------------------
# Dockerfile to build Docker Image for nginx
#
# Made by dumpk1d 26-February-2024
#---------------------------------------------------------------------- 
FROM alpine	

MAINTAINER dumpk1d

RUN	apk update && \
	apk upgrade && \
	apk add --update --no-cache openssl nginx && \
	mkdir /etc/nginx/certificates
	 
EXPOSE 80 443

ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
