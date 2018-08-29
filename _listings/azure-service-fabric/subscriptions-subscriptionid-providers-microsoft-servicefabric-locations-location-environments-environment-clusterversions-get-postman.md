{
  "info": {
    "name": "Azure Service Fabric API Cluster Versions List",
    "_postman_id": "02a94e87-a9d3-4aca-9805-d0ccedc9c8c0",
    "description": "List cluster code versions by location",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "cluster versions",
      "item": [
        {
          "id": "11206811-d680-4b1e-ba0e-1fc52a8bbc86",
          "name": "ClusterVersions_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.ServiceFabric/locations/:location/environments/:environment/clusterVersions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "location",
                  "value": "location",
                  "type": "string"
                },
                {
                  "id": "environment",
                  "value": "environment",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List cluster code versions by location"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd05977a-7a41-4955-8809-711f05334031"
            }
          ]
        }
      ]
    }
  ]
}