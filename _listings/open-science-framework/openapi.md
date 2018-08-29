swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 1
info:
  title: Open Science Framework
  description: osf-provides-free-and-open-source-project-management-support-for-researchers-across-the-entire-research-lifecycle--as-a-collaboration-tool-osf-helps-researchers-work-on-projects-privately-with-a-limited-number-of-collaborators-and-make-parts-of-their-projects-public-or-make-all-the-project-publicly-accessible-for-broader-dissemination--as-a-workflow-system-osf-enables-connections-to-the-many-services-researchers-already-use-to-streamline-their-process-and-increase-efficiency--as-a-flexible-repository-it-can-store-and-archive-research-data-protocols-and-materials--
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
  /files/{file_id}/versions/{version_id}/:
    get:
      summary: Retrieve a file version
      description: |-
        Retrieves the details of a file version
        ####Returns

        Returns a JSON object with a `data` key containing the representation of the requested file, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: files_version_detail
      x-api-path-slug: filesfile-idversionsversion-id-get
      parameters:
      - in: path
        name: file_id
        description: The unique identifier of the file from which you want to retrieve
          versions
      - in: path
        name: version_id
        description: The file version number you want to retrieve
      responses:
        200:
          description: OK
      tags:
      - Files
      - File
      - Versions
      - Version