---
swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 0
info:
  title: Open Science Framework List all file versions
  description: |-
    A paginated list of all file versions.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of 10 file versions. Each resource in the array is a separate file version object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  contact:
    name: OSF
    url: https://osf.io/support
    email: support@osf.io
  version: "2.0"
host: test-api.osf.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{file_id}/versions/:
    get:
      summary: List all file versions
      description: |-
        A paginated list of all file versions.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 file versions. Each resource in the array is a separate file version object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: files_versions
      x-api-path-slug: filesfile-idversions-get
      parameters:
      - in: path
        name: file_id
        description: The unique identifier of the file from which you want to retrieve
          versions
      responses:
        200:
          description: OK
      tags:
      - Files
      - File
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