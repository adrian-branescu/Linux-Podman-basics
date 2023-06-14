FROM nginx:mainline-alpine

# all of these are happening when we build an image/container
# these files/directories are inside the container
# we can see them with docker exec -it $container_id /bin/sh (runs shell on container)


# removes contents from conf.d directory
RUN rm /etc/nginx/conf.d/*

#adding various files in container

#the conf file we use for our server
ADD hello.conf /etc/nginx/conf.d/
#the html file
ADD index.html /usr/share/nginx/html/
#the images directory(containing our image)
ADD images /usr/share/nginx/html/images
