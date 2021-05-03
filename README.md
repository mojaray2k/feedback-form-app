# feedback-form-app

## Docker Commands

### Pass in an env file

```code
docker run -p 3000:8080 -d --rm --env-file ./.env --name feedback-app -v feedback:/app/feedback -v "/Users/amenra/Projects/DOCKER/docker-kubernetes-samples/feedback-form-app:/app:ro" -v /app/temp -v /app/node_modules feedback-node:env
```

### Build with a tag and pass in a variable

```code
docker build -t feedback-node:dev --build-arg DEFAULT_PORT=8080 .
```
