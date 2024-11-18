# FROM node:20 AS builder
# WORKDIR /opt/server
# COPY package.json .
# COPY *.js .
# RUN npm install


# FROM node:20.18.0-alpine3.20
# EXPOSE 8080
# ENV DB_HOST="mysql"
# RUN addgroup -S expense && adduser -S expense -G expense && \
#     mkdir /opt/server && \
#     chown -R expense:expense /opt/server
# WORKDIR /opt/server
# COPY --from=builder /opt/server /opt/server
# USER expense
# CMD ["node", "index.js"]



# Before best practices implemented
FROM node:20
EXPOSE 8080
ENV DB_HOST="mysql"
RUN mkdir /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install  
#All the dependencies will get installed with this command
CMD ["node", "index.js"] 
#after installing all the dependencies we will write system service nothing but running index.js 