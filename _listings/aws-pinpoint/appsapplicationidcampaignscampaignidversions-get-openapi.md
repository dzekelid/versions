---
swagger: "2.0"
x-collection-name: AWS Pinpoint
x-complete: 0
info:
  title: AWS Pinpoint API Campaign Versions List
  version: 1.0.0
  description: Use the GET method to request information about your campaign versions.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/application-id/campaigns/campaign-id/versions:
    get:
      summary: Campaign Versions List
      description: Use the GET method to request information about your campaign versions.
      operationId: getVersonsList
      x-api-path-slug: appsapplicationidcampaignscampaignidversions-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json  A
          JSON response body'
        type: string
        format: string
      - in: query
        name: page-size
        description: The number of entries you want on each page in the response
        type: string
        format: string
      - in: query
        name: token
        description: token
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign Versions
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