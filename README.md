# Implement Simple KONG API Gateway

## How to use

first clone this repository.

### Deno Setup

link documentation installation deno (https://deno.land/manual@v1.28.3/getting_started/installation)

run deno with this command

```
deno run hello-service.ts
```

### Kong Setup

just run this command

```
docker-compose up -d
```

### Try Service Call

```
curl http://localhost:8000/hello
```

### Try Rate API Limiting

```
curl http://localhost:8000/hello
```

Because on the config is setting to 3 hits per minute, so you can try 4 times hitting. And you will get 'API rate limit exceeded'.
