swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 1
info:
  title: AWS ElastiCache API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeCacheEngineVersions:
    get:
      summary: Describe Cache Engine Versions
      description: |-
        Returns a list of the available cache
                    engines and their versions.
      operationId: describeCacheEngineVersions
      x-api-path-slug: actiondescribecacheengineversions-get
      parameters:
      - in: query
        name: CacheParameterGroupFamily
        description: The name of a specific cache parameter group family to return
          details for
        type: string
      - in: query
        name: DefaultOnly
        description: If true, specifies that only the default version of the specified
          engine or engine            and major version combination is to be returned
        type: string
      - in: query
        name: Engine
        description: The cache engine to return
        type: string
      - in: query
        name: EngineVersion
        description: The cache engine version to return
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Engine Versions