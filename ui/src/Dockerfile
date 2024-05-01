FROM node:13.12.0-alpine

# set working directory
WORKDIR /app/
ENV PATH /app/node_modules/.bin:$PATH

# add app
COPY ./ui ./
RUN npm install
RUN npm install react-scripts@5.0.1 -g

# Set environment variables
ENV CHOKIDAR_USEPOLLING=true
ENV WATCHPACK_POLLING=true

# start app
CMD [ "npm" , "start" ]
