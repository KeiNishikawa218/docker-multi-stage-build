# How to start

### normal

##### start container

```
docker compose -f docker-compose-normal.yml build
docker compose -f docker-compose-normal.yml up -d
```

##### access

http://localhost:5173/

### multi stage

##### start container

```
docker compose -f docker-compose-multi-stage.yml build
docker compose -f docker-compose-multi-stage.yml up -d
```

##### access

http://localhost/index.html
