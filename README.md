# Rabbitmq Demo
## How to run
0. Install dependencies
```commandline
pip install -r requirements.txt
```
1. Run RabbitMQ server
```commandline
docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.9-management
```
2. Run the consumer
```commandline
python consumer.py
```
3. Run the producer
```commandline
python producer.py
```