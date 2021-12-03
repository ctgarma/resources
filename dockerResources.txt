Docker resources

# Docker command 

docker --version
docker ps.      /* list all containers */

/* stop a container. */
docker stop <container Id>
  
/* list all volumes */
docker volume ls

/* remove all unused volumes */  
docker volume prune

/* build a docker image */
  docker build --tag <set the image name here>
  
/* running a docker container */
  docker run -d -p 8000:8000 node-docker 
  
  docker run -d -p 8000:8000 --name <name the container here>  <name of the image>
  
/*sample Dockerfile */

FROM node:12.18.1
WORKDIR /app
COPY package.json package.json
COPY package-lock.json package-lock.json
RUN npm install
COPY . .
CMD [ "node", "server.js" ]

  https://www.docker.com/blog/getting-started-with-docker-using-node-jspart-i/
