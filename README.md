## 📨 RabbitMQ Study

A simple lab with Python and RabbitMQ to understand some RabbitMQ fundamentals.

In this project, I only receive and publish messages in the most basic way.


## 🚀 How to run

To run this application you need to follow these instructions:

* Install python3 and docker-compose in your machine.
* In root path of this project, run this follow command in terminal: ``docker-compose up -d``

This command will up a docker container of RabbitMQ in your machine at http://localhost:15672.

User and password on localhost are **guest.**

---



Now, you need to create a Exchange called "data_exchange" and a Queue called "data_queue" in RabbitMQ Management Console.

After creating both, you need to bind your Queue in your Exchange.

Finally, you can run these following comands in terminal (Root path of project):

* `python3 consumer.py` - This command will print the messages that will receive
* `python3 publisher.py` - This command will publish new messages to your Queue.

Now, you can view in terminal the flow of publish and receive message.
