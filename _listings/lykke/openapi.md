swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /home/Version:
    get:
      summary: Get Home Version
      description: Get home version.
      operationId: HomeVersionGet
      x-api-path-slug: homeversion-get
      responses:
        200:
          description: OK
      tags:
      - Home
      - Version