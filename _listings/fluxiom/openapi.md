---
swagger: "2.0"
x-collection-name: Fluxiom
x-complete: 1
info:
  title: Fluxiom API
  description: the-fluxiom-api-allows-you-to-hook-into-fluxiom-and-connect-it-with-other-apps-
  termsOfService: http://www.fluxiom.com/terms
  version: v1
host: '{subdomain}.fluxiom.com'
basePath: /api/{format}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/assets/ID/versions:
    get:
      summary: Get asset versions
      description: Get asset versions
      operationId: get-asset-versions
      x-api-path-slug: apiassetsidversions-get
      responses:
        200:
          description: OK
      tags:
      - Assets
      - Versions
    post:
      summary: Create asset version
      description: Create asset version
      operationId: create-asset-version
      x-api-path-slug: apiassetsidversions-post
      parameters:
      - in: query
        name: comment
        description: comment     tt string
      - in: query
        name: file
        description: file        tt postdata
      responses:
        200:
          description: OK
      tags:
      - Assets
      - Versions
  /api/assets/ID/versions/VID:
    get:
      summary: Get single asset version
      description: Get single asset version
      operationId: get-single-asset-version
      x-api-path-slug: apiassetsidversionsvid-get
      responses:
        200:
          description: OK
      tags:
      - Assets
      - Versions
      - VID
---