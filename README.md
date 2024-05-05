Subir o swagger via docker

SWAGGER EDITOR

https://github.com/swagger-api/swagger-editor

comandos:

docker pull swaggerapi/swagger-editor
docker run -d -p 80:8080 -v $(pwd):/tmp -e SWAGGER_FILE=/tmp/openapi.yaml swaggerapi/swagger-editor

no navegador, acessar o swagger: localhost


SWAGGER UI

https://github.com/swagger-api/swagger-ui

comandos:

docker pull swaggerapi/swagger-ui
docker run -p 80:8080 -e SWAGGER_JSON=/openapi.json -v $(pwd):/tmp swaggerapi/swagger-ui
