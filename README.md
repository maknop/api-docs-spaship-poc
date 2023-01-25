# api-docs-spaship-poc

## Initial Setup
```
spaship env --name=<new-env-name> \
    --url=https://spaship.redhat.com/applications/deploy/developers/<env-name> \
    --apikey=<your-api-key>
```
## Initialize project
```
spaship init -n api-docs-spaship-poc -p /app --single
```

## Build Distribution
Must be defined in `package.yml`
```
npm run build
```

## Build Package Containing Single-Page Application
```
npm pack
```

## Deploy
```
spaship --env=<env>
```