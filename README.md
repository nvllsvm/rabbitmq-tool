# rabbitmq-tool
[![PyPI version](https://img.shields.io/pypi/v/rabbitmq-tool.svg?)](https://pypi.python.org/pypi/rabbitmq-tool/)

A RabbitMQ CLI

**Features**:
- manage bindings
- inspect exchanges and queues
- show all exchanges and queues
- create and delete exchanges and queues

## Why not use one of the existing RabbitMQ CLI's?
Honestly, I don't remember why I wrote this instead of using an existing tool. 🤷

## Installation
```
pip install rabbitmq-tool
```

## Usage Examples
See `--help` for more information.

### Create exchange
```
$ rabbitmq-tool --url http://localhost:15672 --username guest create-exchange myexchange

```

### Create queue
```
$ rabbitmq-tool --url http://localhost:15672 --username guest create-queue myqueue
```

### Bind exchange and queue
```
$ rabbitmq-tool --url http://localhost:15672 --username guest bind --exchange myexchange --queue myqueue --routing '#'
```
