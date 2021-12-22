# Node Rabbitmq Demo

## Setup
### Install package
```sh 
$ npm install

$ brew update
$ brew install rabbitmq

$ export PATH=$PATH:/usr/local/sbin

$ brew services start rabbitmq
$ rabbitmq-server
```

```sh
$ node ./part_1/send.js
$ node ./part_1/receive.js

$ rabbitmqctl list_queues
```

```sh
$ node ./part_2/worker.js
$ node ./part_2/worker.js
$ node ./part_2/new_task.js // 1
$ node ./part_2/new_task.js // 2
$ node ./part_2/new_task.js // 3
$ node ./part_2/new_task.js // 4
$ node ./part_2/new_task.js // 5

$ rabbitmqctl list_queues
```

## Ref
- [Install RabbitMQ](https://www.rabbitmq.com/install-homebrew.html)
- [RabbitMQ CLI](https://www.rabbitmq.com/cli.html)
- [Tutorial Part 1](https://www.rabbitmq.com/tutorials/tutorial-one-javascript.html)
- [Tutorial Part 2](https://www.rabbitmq.com/tutorials/tutorial-two-javascript.html)
