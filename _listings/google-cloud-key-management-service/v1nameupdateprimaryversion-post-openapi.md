---
swagger: "2.0"
x-collection-name: Google Cloud Key Management Service
x-complete: 0
info:
  title: Google Cloud Key Management Service API Update Version
  description: Update the version of a CryptoKey that will be used in Encrypt
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudkms.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:updatePrimaryVersion:
    post:
      summary: Update Version
      description: Update the version of a CryptoKey that will be used in Encrypt
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.updatePrimaryVersion
      x-api-path-slug: v1nameupdateprimaryversion-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the CryptoKey to update
      responses:
        200:
          description: OK
      tags:
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