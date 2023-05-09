docker run -d -it --name Dependencies ubuntu sh -c "echo 'Input website:'; read website; echo 'Searching..'; sleep 1; curl http://$website;"

docker exec -it Dependencies bash

apt-get update; apt-get install curl

docker attach Dependencies

helsinki.fi
