# Job Hunter

### Services Links

| Component | Link |
| ------ | ------ |
| Job Hunter API Gateway | https://github.com/job-hunter-pad/job-hunter-api-gateway |
| Job Hunter Frontend | https://github.com/job-hunter-pad/job-hunter-frontend |
| Job Hunter Authentication Service | https://github.com/job-hunter-pad/job-hunter-authentication |
| Job Hunter Email Service | https://github.com/job-hunter-pad/job-hunter-emailservice |
| Job Hunter Employer Service | https://github.com/job-hunter-pad/job-hunter-employer-service |
| Job Hunter Freelancer Service | https://github.com/job-hunter-pad/job-hunter-freelancer-service |
| Job Hunter Payment Service | https://github.com/job-hunter-pad/job-hunter-payment-service | 


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

Environment Variables are stored in a `.env` file in the same folder with the `docker-compose.yml` file

### Kafka

- KAFKA_BIND_MOUNT

### Zookeeper

- ZOOKEEPER_DATA_BIND_MOUNT
- ZOOKEEPER_LOGS_BIND_MOUNT

### MongoDB

- MONGODB_USERNAME
- MONGODB_PASSWORD
- MONGODB_BIND_MOUNT

### Env File Example
```
MONGODB_BIND_MOUNT=./persistance/mongodb

ZOOKEEPER_DATA_BIND_MOUNT=./persistance/zookeeper/data
ZOOKEEPER_LOGS_BIND_MOUNT=./persistance/zookeeper/logs
 
KAFKA_BIND_MOUNT=./persistance/kafka
```

