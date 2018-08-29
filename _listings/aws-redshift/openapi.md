swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 1
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeClusterVersions:
    get:
      summary: Describe Cluster Versions
      description: Returns descriptions of the available Amazon Redshift cluster versions.
      operationId: describeClusterVersions
      x-api-path-slug: actiondescribeclusterversions-get
      parameters:
      - in: query
        name: ClusterParameterGroupFamily
        description: The name of a specific cluster parameter group family to return
          details            for
        type: string
      - in: query
        name: ClusterVersion
        description: The specific cluster version to return
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters