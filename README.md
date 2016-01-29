# rabbitmq-mongodb

use:

```
$ docker run -d \
  --restart=always \
  --name rabbitmq-mongodb \
  -e AMQPHOST=amqp://<RABBITMQ_HOSTNAME> \
  -e MONGODB=mongodb://<MONGODB_HOSTNAME>/<MONGODB_DATABASE> \
  -e MONGOCOLLECTION=<MONGODB_COLLECTION> \
  -e TRANSLATECONTENT=true \
  -e QUEUENAME=xxqueue \
  bowwow/amqp-mongo
```
