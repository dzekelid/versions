---
swagger: "2.0"
x-collection-name: Azure Service Fabric
x-complete: 1
info:
  title: ServiceFabricManagementClient
  version: 1.0.0
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
---