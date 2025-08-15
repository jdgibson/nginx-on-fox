# nginx-on-fox

### Run for Debugging

To start for debugging:

```
docker compose up
```

### To Run in Production.

To run in background

```
docker compose up -d
```

## Viewing Error Logs

To view the error logs from the nginx Docker container:

### View live logs (real-time)
```
docker compose logs -f
```

### View logs for a specific service (if you have multiple services)
```
docker compose logs -f nginx
```

### View recent logs without following
```
docker compose logs
```

### View logs with timestamps
```
docker compose logs -t
```

### View only the last N lines of logs
```
docker compose logs --tail=50
```

### Alternative: Direct docker logs command
If you need to use the container name directly:
```
docker logs -f <container_name>
```

To find the container name, use:
```
docker ps
```


