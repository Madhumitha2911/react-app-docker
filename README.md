# React in docker

## Run react Application as docker

### TASK:
1. Clone this repository
2. Create a Dockerfile
    1. with node image of specific version
    2. declare working directory as /app
    3. copy package.json and package.lock.json to working directory
    4. build project : `npm install`
    5. copy project files into image working directory and create `.dockerignore` file to exclude `node modules` during build process
    6. Expose 3000 port
    7. add  command to start the react project : `npm start`
3. Build the image with version tag.
4. Run the container with port forwarding 3001:3000 
5. Hit the localhost:3001 to view the app
6. Tag the image with your Docker-ID (create a docker-id if not available) example `<my-docker-id>/<repo-name>:<tag-name>`
7. Login docker hub `docker login`
8. Push the docker image to the Docker hub `docker push <my-docker-id>/<repo-name>:<tag-name>`
