# Job Hunter

### Services Links

| Component | Link|
| ------ | ------ |
| Job Hunter API Gateway | https://github.com/job-hunter-pad/job-hunter-api-gateway |
| Job Hunter Frontend | https://github.com/job-hunter-pad/job-hunter-frontend |
| Job Hunter Authentication Service | https://github.com/job-hunter-pad/job-hunter-authentication |
| Job Hunter Email Service | https://github.com/job-hunter-pad/job-hunter-emailservice |


## How to Build

### Update Docker Compose Images

```
docker-compose pull
```

### Build Docker Compose 

```
docker-compose up
```
### Remove Containers

```
docker-compose down
```

## Environment Variables

They are stored in a `.env` file

### Kafka

- KAFKA_BIND_MOUNT

> Example: 
> `KAFKA_BIND_MOUNT=./persistance/kafka`

### Zookeeper

- ZOOKEEPER_DATA_BIND_MOUNT
- ZOOKEEPER_LOGS_BIND_MOUNT

> Example:
> 
> `ZOOKEEPER_DATA_BIND_MOUNT=./persistance/zookeeper/data`
> 
> `ZOOKEEPER_LOGS_BIND_MOUNT=./persistance/zookeeper/logs`

### MongoDB

- MONGODB_USERNAME
- MONGODB_PASSWORD
- MONGODB_BIND_MOUNT

> Example:
> `MONGODB_BIND_MOUNT=./persistance/mongodb`

