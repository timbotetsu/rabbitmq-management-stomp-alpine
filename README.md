# RabbitMQ based on Alpine with management and STOMP plugin

This is a docker image based on [offical RabbitMQ image](https://hub.docker.com/_/rabbitmq/), which could accept environment variables as the offical image, but with [STOMP plugin](https://www.rabbitmq.com/stomp.html) installed.

# Usage

```
$ docker run -d --name some-rabbitmq -p 5672:5672 -p 16572:16572 -p 61613:61613 timbotetsu/rabbitmq-management-stomp-alpine
```

port 5672 for AMQP connection

port 16572 for management Portal

port 61613 for STOMP connections