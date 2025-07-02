# Docker-Python-Repo
Dockerised Python code

FROM python:latest
WORKDIR /usr/app/src
COPY helloworld.py ./
CMD [ "python", "./helloworld.py"] 

 mkdir project
 pwd
 cd project
 pwd
 touch dockerfile
 tree
 sudo tree
 sudo yum install tree
 sudo tree -v
 touch helloworld.py
 tree
 nano helloworld.py
 nano dockerfile
 cat dockerfile
 python3 helloworld.py
 sudo docker login
 sudo docker build -t avinashtale99/pythonhelloworld .
 sudo docker images
 sudo docker run b65eaec46c1f
 sudo docker container ls
 sudo docker ps -a
 sudo docker push b65eaec46c1f
 sudo docker push avinashtale99/pythonhelloworld
