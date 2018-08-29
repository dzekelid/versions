---
swagger: "2.0"
x-collection-name: AWS Lambda
x-complete: 0
info:
  title: AWS Lambda API Publish Version
  version: 1.0.0
  description: Publishes a version of your function from the current snapshot of $LATEST.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PublishVersion:
    get:
      summary: Publish Version
      description: Publishes a version of your function from the current snapshot
        of $LATEST.
      operationId: publishVersion
      x-api-path-slug: actionpublishversion-get
      parameters:
      - in: query
        name: FunctionName
        description: The Lambda function name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Version
  /?Action=ListVersionsByFunction:
    get:
      summary: List Versions By Function
      description: List all versions of a function.
      operationId: listVersionsByFunction
      x-api-path-slug: actionlistversionsbyfunction-get
      parameters:
      - in: query
        name: FunctionName
        description: Function name whose versions to list
        type: string
      - in: query
        name: Marker
        description: Optional string
        type: string
      - in: query
        name: MaxItems
        description: Optional integer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Functions
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