---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get Home Version
  version: 1.0.0
  description: Get home version.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---