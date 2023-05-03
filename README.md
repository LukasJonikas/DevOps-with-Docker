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



