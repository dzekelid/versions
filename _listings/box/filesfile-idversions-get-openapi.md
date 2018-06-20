---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box View Versions
  description: If there are previous versions of this file, this method can be used
    to retrieve information about the older versions. (Versions are only tracked for
    Box users with premium accounts.)
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{FILE_ID}/versions:
    get:
      summary: View Versions
      description: If there are previous versions of this file, this method can be
        used to retrieve information about the older versions. (Versions are only
        tracked for Box users with premium accounts.)
      operationId: getFileVersions
      x-api-path-slug: filesfile-idversions-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: FILE_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
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