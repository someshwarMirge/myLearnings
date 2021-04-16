##__Docker Commands:__

- __PULL :__ `docker pull <container_name>`
- __RUN:__ `docker run <name/id>`
- __LIST:__ `docker ps / docker ps -a / docker ps -l  <name/id>`
- __START:__`docker start <name/id>`
- __STOP:__ `docker stop <name/id>`
- __REMOVE:__ `docker rm <name/id>`
- __HELP:__ `docker <option> help : docker run help/ docker start help`
- __COMMIT :__ `docker commit -m "What you did to the image" -a "Author Name" container_id repository/new_image_name
	-m = for message 
	-a = to specify author 
	repository = repository name from docker hub / generally username 
	new_image_name= any name that you want`
- __LOGIN:__ `docker login -u docker-registry-username`
- __TAG:__ `docker tag sammy/ubuntu-nodejs docker-registry-username/ubuntu-nodejs`
- __PUSH:__ `docker push docker-registry-username/docker-image-name ::: docker push sammy/ubuntu-nodejs`