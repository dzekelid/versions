---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 GET Bucket Object versions
  version: 1.0.0
  description: You can use the versions subresource to list metadata about all ofthe
    versions of objects in a bucket
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?versions:
    get:
      summary: GET Bucket Object versions
      description: You can use the versions subresource to list metadata about all
        ofthe versions of objects in a bucket
      operationId: get-bucket-object-versions
      x-api-path-slug: versions-get
      parameters:
      - in: query
        name: delimiter
        description: A delimiter is a character that you specify to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: key-marker
        description: Specifies the key in the bucket that you want to start listingtttttttttfrom
      - in: query
        name: max-keys
        description: Sets the maximum number of keys returned in the response body
      - in: query
        name: prefix
        description: Use this parameter to select only those keys that begin withtttttttttthe
          specified prefix
      - in: query
        name: version-id-marker
        description: Specifies the object version you want to start listing from
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Object
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