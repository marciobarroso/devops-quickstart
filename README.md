# devops-quickstart

# BUILD
docker build -t docker/jenkins:latest .

# RUN
docker run -p 8080:8080 \
  -v /var/run/docker.sock:/var/run/docker.sock \
  --name jenkins \
  docker/jenkins:latest

# ONLINE SETUP
Go to localhost:8080 and install the sugested plugins

# CONNECT
docker exec -it -u root jenkins bash  
