---
swagger: "2.0"
x-collection-name: IBM Cloud
x-complete: 0
info:
  title: IBM Containers List latest API version
  description: This endpoint retrieves a list of all microservices that are used in
    the IBM Containers service with their current build version. This method does
    not require authentication.
  version: 3.0.0
host: containers-api.ng.bluemix.net
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /containers/version:
    get:
      summary: List latest API version
      description: This endpoint retrieves a list of all microservices that are used
        in the IBM Containers service with their current build version. This method
        does not require authentication.
      operationId: this-endpoint-retrieves-a-list-of-all-microservices-that-are-used-in-the-ibm-containers-service-with
      x-api-path-slug: containersversion-get
      responses:
        200:
          description: OK
      tags:
      - Containers
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