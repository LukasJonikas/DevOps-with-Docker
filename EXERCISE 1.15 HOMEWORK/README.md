https://hub.docker.com/repository/docker/lukasjonikas01/prometheus/general

To get he images: docker pull lukasjonikas01/prometheus:prom

Run command: docker run -it -d -p 9090:9090 lukasjonikas01/prometheus

After running commands an instance of prometheus should be available on localhost:9090

Default yml file that was used to build the image can be found at https://github.com/vegasbrianc/prometheus/blob/master/docker-compose.yml
