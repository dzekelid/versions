---
swagger: "2.0"
x-collection-name: Azure Service Fabric
x-complete: 0
info:
  title: Azure Service Fabric API Cluster Versions List
  version: 1.0.0
  description: List cluster code versions by location
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/providers/Microsoft.ServiceFabric/locations/{location}/environments/{environment}/clusterVersions
  : get:
      summary: Cluster Versions List
      description: List cluster code versions by location
      operationId: ClusterVersions_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-servicefabriclocationslocationenvironmentsenvironmentclusterversions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Cluster Versions
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