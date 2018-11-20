# specify a base image
FROM node:alpine

WORKDIR /usr/app

# Install dependencies
COPY ./package.json ./
RUN npm install
COPY ./ ./

# default command
CMD ["npm", "start"]

# docker build -t mattyfew/simpleweb .          // build and tag... what does the . mean?
# docker run -p 8080:8080 mattyfew/simpleweb    // map port
# docker run -it mattyfew/simpleweb sh          // open prompt to look at files
# docker exec -it a2d45aaf86fe sh