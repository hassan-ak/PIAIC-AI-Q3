FROM alpine
LABEL maintainer="johndoe@yahoo.com"
RUN apk add --update nodejs npm
COPY . /src
WORKDIR /src
RUN npm install
ENV CREATEDBY="Hassan Ali Khan"
EXPOSE 8080
ENTRYPOINT ["node", "./app.js"]
