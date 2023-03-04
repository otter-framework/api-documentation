# API Documentation For Otter Framework

View REST API documentation [here](https://otter-framework.github.io/api-documentation/)

### Update API specification
- Clone or pull this repo
- Refer [OpenAPI specification](https://oai.github.io/Documentation/start-here.html) and update `openapi.yml` when changes needed. To make sure Otter API is following OpenAPI spec, use [Redoc](https://github.com/Redocly/redoc) to lint the YAML file before building the documentation:
```
redocly lint openapi.yml
```

### Build API documentation
After updating `openapi.yml`, first run
```
redocly build-docs openapi.yml --output=index.html --title="Otter API"
```
Then push updates to the repo.
