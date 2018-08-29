---
swagger: "2.0"
info:
  title: OpenCorporates Versions
  description: nThis returns the current version of the API and supported versions
  termsOfService: https://opencorporates.com/info/licence
  version: v.04
host: api.opencorporates.com
basePath: v0.4/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /versions:
    get:
      summary: Versions
      description: nThis returns the current version of the API and supported versions
      operationId: versions
      responses:
        200:
          description: OK
      tags:
      - businesses
      - versions
definitions: []
x-collection-name: OpenCorporates
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