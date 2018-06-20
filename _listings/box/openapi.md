---
swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
  description: the-box-content-api-gives-you-access-to-secure-content-management-and-content-experience-features-for-use-in-your-own-app--it-strives-to-be-restful-and-is-organized-around-the-main-resources-youre-familiar-with-from-the-box-web-interface-
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
---