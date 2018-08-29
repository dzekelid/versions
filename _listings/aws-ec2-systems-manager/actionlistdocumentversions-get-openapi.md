---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API List Document Versions
  version: 1.0.0
  description: List all versions for a document.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListDocumentVersions:
    get:
      summary: List Document Versions
      description: List all versions for a document.
      operationId: listDocumentVersions
      x-api-path-slug: actionlistdocumentversions-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: Name
        description: The name of the document about which you want version information
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Document
      - Versions
  /?Action=UpdateDocumentDefaultVersion:
    get:
      summary: Update Document Default Version
      description: Set the default version of a document.
      operationId: updateDocumentDefaultVersion
      x-api-path-slug: actionupdatedocumentdefaultversion-get
      parameters:
      - in: query
        name: DocumentVersion
        description: The version of a custom document that you want to set as the
          default version
        type: string
      - in: query
        name: Name
        description: The name of a custom document that you want to set as the default
          version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
      - Default
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