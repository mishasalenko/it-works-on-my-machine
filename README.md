# it-works-on-my-machine

## Run Full Stack (Backend + Frontend)
```bash
docker compose -f docker-compose.yml up --build
```

### Start Backend Services

```bash
docker compose -f docker-compose.backend.yml up --build
```

### Start frontend Services
```bash
docker compose -f docker-compose.frontend.yml up --build
```

### Stop and Remove Volumes
```bash
docker compose -f docker-compose.backend.yml down -v
```

### Delete Redis key videos
```bash
docker exec -it docker-redis-### redis-cli DEL videos
```