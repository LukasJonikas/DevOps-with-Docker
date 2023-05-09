docker build . -t frontend

dockerbuild . -t backend

docker run -it -d -p 5000:5000 frontend

docker run -it -d -p 8080:8080 backend
