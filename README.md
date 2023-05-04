# DevOps-with-Docker

EXERCISE 1.1: GETTING STARTED

Output:

![image](https://user-images.githubusercontent.com/132380151/235957786-8d125da8-4454-4353-adb6-5c5714dc0db6.png)

EXERCISE 1.2: CLEANUP

docker ps -as output:

![image](https://user-images.githubusercontent.com/132380151/235958822-736fc3cd-d0ce-41b1-8d1d-006bfb71bbcb.png)

docker images output:

![image](https://user-images.githubusercontent.com/132380151/235959123-1c21ffc0-e41d-47ec-adb6-465779d13711.png)

EXERCISE 1.3: SECRET MESSAGE

Secret message: 'You can find the source code here: https://github.com/docker-hy'

Commands used:

docker run -d -it devopsdockeruh/simple-web-service:ubuntu

docker exec -it quirky_franklin bash

tail -f text.log

EXERCISE 1.4: MISSING DEPENDENCIES

docker run -d -it --name Dependencies ubuntu sh -c "echo 'Input website:'; read website; echo 'Searching..'; sleep 1; curl http://$website;"

docker exec -it Dependencies bash

apt-get update; apt-get install curl

docker attach Dependencies

helsinki.fi

EXERCISE 1.5: SIZES OF IMAGES

![image](https://user-images.githubusercontent.com/132380151/236217234-8efdc029-5207-4c75-b20f-1ea7bea6e745.png)

![image](https://user-images.githubusercontent.com/132380151/236220386-b775ae37-8d39-4574-98c0-2fb46d5f9eaa.png)

EXERCISE 1.6: HELLO DOCKER HUB

https://hub.docker.com/r/devopsdockeruh/pull_exercise

![image](https://user-images.githubusercontent.com/132380151/236250912-a597082d-ca92-4558-82ef-17fed44bdeda.png)


EXERCISE 1.7: IMAGE FOR SCRIPT

FROM ubuntu:20.04

WORKDIR /usr/src/app

RUN apt-get update; apt-get install curl -y;

COPY thescript.sh .

CMD ./thescript.sh

EXERCISE 1.8: TWO LINE DOCKERFILE

Dockerfile:

FROM devopsdockeruh/simple-web-service:alpine

CMD server

Commands:

docker run webserver

EXERCISE 1.9: VOLUMES

cat text.log

EXERCISE 1.10: PORTS OPEN

docker run -d -it -p 8080:8080 devopsdockeruh/simple-web-service server

curl http://localhost:8080





