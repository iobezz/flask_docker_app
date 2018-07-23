# как запускать
# sudo docker-compose --project-name mongo-client -f docker-compose.yml up --build -d
# sudo docker-compose --project-name mongo-client -f docker-compose.yml run --rm mongo-client
# /usr/bin/mongo -host $APP_MONGO_HOST -port $APP_MONGO_PORT

FROM alpine:edge

RUN echo "http://dl-8.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories

RUN apk update && apk upgrade && apk --no-cache --update-cache add mongodb su-exec curl mongodb-tools nano


COPY ./src/* /home/
