swagger: "2.0"
x-collection-name: Code.gov
x-complete: 1
info:
  title: Code.gov API
  description: code-gov-api-documentation--while-using-this-documentation-locally-please-choose-to-
  version: 1.0.0
host: api.code.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /version:
    get:
      summary: Get the version of this API
      description: Get the version of this api.
      operationId: getVersion
      x-api-path-slug: version-get
      responses:
        200:
          description: OK
      tags:
      - Code
      - Version