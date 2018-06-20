---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Delete Old Version
  description: Discards a specific file version to the trash. (Depending on the enterprise
    settings for this user, the item will either be actually deleted from Box or moved
    to the trash.)
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
  /files/{FILE_ID}/versions/current:
    post:
      summary: Promote Version
      description: If there are previous versions of this file, this method can be
        used to promote one of the older versions to the top of the stack. This actually
        mints a copy of the old version and puts it on the top of the versions stack.
        The file will have the exact same contents, the same SHA1/etag, and the same
        name as the original. Other properties such as comments do not get updated
        to their former values.
      operationId: promotoeFileVersion
      x-api-path-slug: filesfile-idversionscurrent-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
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
      - Current
  /files/{FILE_ID}/versions/{VERSION_ID}:
    delete:
      summary: Delete Old Version
      description: Discards a specific file version to the trash. (Depending on the
        enterprise settings for this user, the item will either be actually deleted
        from Box or moved to the trash.)
      operationId: deleteFileVersion
      x-api-path-slug: filesfile-idversionsversion-id-delete
      parameters:
      - in: path
        name: FILE_ID
      - in: header
        name: If-Match
        description: The etag of the file
      - in: path
        name: VERSION_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
      - Versions
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