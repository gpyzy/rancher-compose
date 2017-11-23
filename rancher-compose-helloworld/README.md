# rancher-compose-helloworld
This repository demos how to use rancher-compose to create a hello world container.
the docker image that be used in this demo is from https://hub.docker.com/r/kitematic/hello-world-nginx

## Option 1 - Use Docker Remote API in docker-compose.yml
In this link https://forums.rancher.com/t/rancher-compose-and-local-dockerfile-using-build/612 it describes how to use Docker Remote API in docker-compose and rancher-compose to create a container. This demo doesn't go with this solution.
TODO - A seperate demo will be created and go with this solution.

## Option 2 - use image parameter in docker-compose.yml
This demo goes with this solution


# Register additional node example
mac-ranch -r 'sudo docker run --rm --privileged -v /var/run/docker.sock:/var/run/docker.sock -v ${HOME}/var/lib/rancher:/var/lib/rancher rancher/agent:v1.2.6 http://192.168.64.29:8080/v1/scripts/B9A82CDCDC5C95F49999:1483142400000:Ty4hwDYyR4oJxdezSTRghsKw44' -M 5000 -n 1 -b http://localhost:8001/boot2docker.iso -u https://registry.docker-cn.com rs

mac-ranch -c -n 1 -M 5000 -b http://localhost:8001/boot2docker.iso -u http://registry.docker-cn.com rs

