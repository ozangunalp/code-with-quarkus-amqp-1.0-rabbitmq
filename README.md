# code-with-quarkus-amqp-1.0-rabbitmq

Example project using RabbitMQ as AMQP 1.0 broker.

First start the RabbitMQ configured with AMQP 1.0 plugin defined in `docker-compose.yml`:

```bash
docker compose up
```

Then start the application in dev mode:

```bash
quarkus dev
```

Because the docker compose service contains the label `quarkus-dev-service-amqp=amqp`, the AMQP dev service will pick it up and configure the application correctly in dev mode, instead of creating a new dev service container.
