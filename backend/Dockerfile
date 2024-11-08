FROM node:20
EXPOSE 8080
ENV DB_HOST="mysql"
#opt- optional
RUN mkdir /opt/server 

#moving to the directory
WORKDIR /opt/server

#we have placed package.json and all the js files in /opt/server
COPY package.json .
COPY *.js .

#installed 
RUN npm install

#running it
CMD ["node","index.js"]


