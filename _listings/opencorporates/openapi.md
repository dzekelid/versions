swagger: "2.0"
x-collection-name: OpenCorporates
x-complete: 1
info:
  title: OpenCorporates
  description: the-api-for-managing-opencorporates-data-
  termsOfService: https://opencorporates.com/info/licence
  version: v.04
host: api.opencorporates.com
basePath: v0.4/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /versions:
    get:
      summary: Versions
      description: nThis returns the current version of the API and supported versions
      operationId: versions
      x-api-path-slug: versions-get
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Versions