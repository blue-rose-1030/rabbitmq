# RabbitMQ simple operations with Python

To successfully use the code you will need a running RabbitMQ server.

## Requirements

To run this code you need to install the `pika` package version `1.0.0` or later. To install it, run

    python -m pip install pika

You may first need to run

    easy_install pip


## Code

- Simple messaging:

    send.py receive.py


- Work Queues:

    new_task.py worker.py


- Publish/Subscribe:

    receive_logs.py emit_log.py "info: This is the log message"


- Routing:

    receive_logs_direct.py info emit_log_direct.py info "The message"


- Topics:

    receive_logs_topic.py "*.rabbit" emit_log_topic.py red.rabbit Hello


- RPC:

    rpc_server.py rpc_client.py
