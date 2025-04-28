# swagger-editor-local
swagger-editor Docker config for testing a local API while avoiding CORS issues

Runs Nginx to forward the swagger-editor container and local API(s) out the same http://localhost/ port so the browser doesn't complain about CORS.  

I'm really only doing this so the "Try it out" button works in swagger-editor without adding additional headers to the API(s).

## Prerequisites
Any recent version of Docker

## Configuration
Add servers and endpoints you need to nginx.conf.

## Run
```sh
docker compose up
```

# Caveats
Only for local testing.
Do not use this for network services without setting up https.
