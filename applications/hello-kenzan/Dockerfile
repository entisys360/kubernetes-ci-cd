FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html
COPY DockerFileEx.jpg /usr/share/nginx/html/DockerFileEx.jpg

EXPOSE 80

#
# TODO:  Figure out how to use values.yaml to inject the appropriate startup CMD based on *something* at build time.
# The below command works beautifully if you do NOT mount web ROOT as a local disk in the container,
# as each container will then have their own container ID in their respective index.html file..
#
#CMD sleep 1 ; echo "Container hostname = $HOSTNAME"  >> index.html ; while true ; do sleep 10 ; done
