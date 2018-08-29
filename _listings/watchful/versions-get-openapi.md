---
swagger: "2.0"
x-collection-name: Watchful
x-complete: 0
info:
  title: Watchful Get List Of Versions
  description: ""
  version: 1.0.0
host: watchful.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /versions:
    get:
      summary: Get List Of Versions
      description: ""
      operationId: getVersions
      x-api-path-slug: versions-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      responses:
        200:
          description: OK
      tags:
      - Versions
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