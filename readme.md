## Redis
One of the most popular nosql key-value dbs.

## Features
- key-value
- follows BASE transaction model

## Docker
1. Pull the image
```
sudo docker pull redis
```
2. Run the image
```
sudo docker run --network "host" -p 6379:6379 -v "/var/lib/redis-data":"/data" -d --name redis redis redis-server
``` 
Setting host for network parameter is needed.

## Connection
Firstly, install redis dependencies
```
sudo apt install redis
```
Then, use either redis-cli to log in:
```
redis-cli -h hostname (if not runing on local) -p 6379 (if specified different port)
```

## Hostname parameter configuration depending on the server
Please, follow same logic as per postgres configuration: https://github.com/ibasa14/postgreSQL-Tutorial

## GUI
The redis supported GUI tool is: RedisInsight