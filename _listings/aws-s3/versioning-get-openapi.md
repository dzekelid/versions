---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 GET Bucket versioning
  version: 1.0.0
  description: This implementation of the GET operation uses theversioning subresource
    to return the versioning state of abucket
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
  /?list-type=2:
    get:
      summary: GET Bucket (List Objects) Version 2
      description: This implementation of the GET operation returns some or all (up
        to 1,000) ofthe objects in a bucket
      operationId: get-bucket-list-objects-version-2
      x-api-path-slug: listtype2-get
      parameters:
      - in: query
        name: continuation-token
        description: When the Amazon S3 response to this API call is truncated (that
          is, IsTruncated responsetttttttttelement value is true), the response also
          includes thettttttttttNextContinuationToken element, the value of whichtttttttttyou
          can use in the next request as thettttttttttcontinuation-token to list the
          next settttttttttof objects
      - in: query
        name: delimiter
        description: A delimiter is a character you use to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: fetch-owner
        description: By default, the API does not return the Owner information in
          the response
      - in: query
        name: list-type
        description: Version 2 of the API requires this parameter and you must set
          its value to 2
      - in: query
        name: max-keys
        description: Sets the maximum number of keys returned in the response body
      - in: query
        name: prefix
        description: Limits the response to keys that begin with the specifiedtttttttttprefix
      - in: query
        name: start-after
        description: If you want the API to return key names after a specifictttttttttobject
          key in your key space, you can add this parameter
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - (List
      - Objects)
      - Version
      - "2"
  /?versioning:
    get:
      summary: GET Bucket versioning
      description: This implementation of the GET operation uses theversioning subresource
        to return the versioning state of abucket
      operationId: get-bucket-versioning
      x-api-path-slug: versioning-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Versioning
    put:
      summary: PUT Bucket versioning
      description: This implementation of the PUT operation uses theversioning subresource
        to set the versioning state of anexisting bucket
      operationId: put-bucket-versioning
      x-api-path-slug: versioning-put
      parameters:
      - in: header
        name: x-amz-mfa
        description: The value is the concatenation of the authenticationtttttttttdevices
          serial number, a space, and the value displayed on yourtttttttttauthentication
          device
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Versioning
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