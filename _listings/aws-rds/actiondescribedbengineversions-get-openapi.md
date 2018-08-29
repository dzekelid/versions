---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Describe D B Engine Versions
  version: 1.0.0
  description: Returns a list of the available DB engines.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeDBEngineVersions:
    get:
      summary: Describe D B Engine Versions
      description: Returns a list of the available DB engines.
      operationId: describedbengineversions
      x-api-path-slug: actiondescribedbengineversions-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The name of a specific DB parameter group family to return details
          for
        type: string
      - in: query
        name: DefaultOnly
        description: Indicates that only the default version of the specified engine
          or engine and major version combination is returned
        type: string
      - in: query
        name: Engine
        description: The database engine to return
        type: string
      - in: query
        name: EngineVersion
        description: The database engine version to return
        type: string
      - in: query
        name: Filters.Filter.N
        description: Not currently supported
        type: string
      - in: query
        name: ListSupportedCharacterSets
        description: If this parameter is specified           and the requested engine
          supports the CharacterSetName parameter for CreateDBInstance,           the
          response includes a list of supported character sets for each engine version
        type: string
      - in: query
        name: ListSupportedTimezones
        description: If this parameter is specified             and the requested
          engine supports the TimeZone parameter for CreateDBInstance,             the
          response includes a list of supported time zones for each engine version
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Engines
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