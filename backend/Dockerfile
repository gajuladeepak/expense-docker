

#before best practices implemented
# FROM node:20
# EXPOSE 8080
# ENV DB_HOST="mysql"
# #opt- optional
# RUN mkdir /opt/server 

# #moving to the directory
# WORKDIR /opt/server

# #we have placed package.json and all the js files in /opt/server
# COPY package.json .
# COPY *.js .

# #installed 
# RUN npm install

# #running it
# CMD ["node","index.js"]



#session 47

FROM node:20.18.0-alpine3.20
EXPOSE 8080
ENV DB_HOST="mysql"
RUN addgroup -S expense && adduser -S appuser -G expense
#opt- optional
RUN mkdir /opt/server.
RUN chown -R expense:expense /opt/server

#moving to the directory
WORKDIR /opt/server

#we have placed package.json and all the js files in /opt/server
COPY package.json .
COPY *.js .

#installed 
RUN npm install
USER expense
#running it
CMD ["node","index.js"]





