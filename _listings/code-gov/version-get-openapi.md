---
swagger: "2.0"
x-collection-name: Code.gov
x-complete: 0
info:
  title: Code.gov Get the version of this API
  description: Get the version of this api.
  version: 1.0.0
host: api.code.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /version:
    get:
      summary: Get the version of this API
      description: Get the version of this api.
      operationId: getVersion
      x-api-path-slug: version-get
      responses:
        200:
          description: OK
      tags:
      - Code
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