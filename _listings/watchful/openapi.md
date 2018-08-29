swagger: "2.0"
x-collection-name: Watchful
x-complete: 1
info:
  title: Watchful
  description: watchful-resulted-from-the-need-for-a-single-unified-dashboard-to-easily-monitor-all-of-the-web-sites-in-our-portfolios--after-years-of-evolution-our-solution-has-matured-into-a-simple-complete-and-professional-service--
  version: 1.0.0
host: watchful.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /versions:
    get:
      summary: Get List Of Versions
      description: ""
      operationId: getVersions
      x-api-path-slug: versions-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      responses:
        200:
          description: OK
      tags:
      - Versions
  /versions/{id}:
    get:
      summary: Find A Version By ID
      description: ""
      operationId: getVersion
      x-api-path-slug: versionsid-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by commas: name,id'
      - in: path
        name: id
        description: ID of version that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Versions
      - Id