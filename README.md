# docker-compose-redis-node-app
Simple Node.js app with Redis in Docker

1. Dockerfile

The Dockerfile defines the runtime for a Node.js application in a Docker container. This script uses the official node:alpine image by copying the package.json files and the application source code, then installing the dependencies and launching the application using the npm start command.

2. package.json

The package.json file contains information about the dependencies of a Node.js application. The start script starts the HTTP server on port 8081.

3. index.js

The index.js file is the source code of the Node.js application. The application uses the Express framework, creates a connection to the Redis server and supports one GET.

4. docker-compose.yml

The docker-compose.yml file defines two services: redis-server and node-app. The redis-server service uses the official Redis image and the node-app service uses the local configuration described in the Dockerfile. 
