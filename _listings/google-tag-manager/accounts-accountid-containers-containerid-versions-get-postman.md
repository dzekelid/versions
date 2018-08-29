{
  "info": {
    "name": "Google Tag Manager API Get Container Versions",
    "_postman_id": "45149d16-0d2e-44a4-bbf7-1a34485cbcd3",
    "description": "Lists all Container Versions of a GTM Container.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "containers",
      "item": [
        {
          "id": "6ef3bf8d-fd4f-4b8f-b548-756772dba0ae",
          "name": "tagmanager.accounts.containers.versions.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tagmanager",
                "v1",
                "accounts/:accountId/containers/:containerId/versions"
              ],
              "query": [
                {
                  "key": "headers",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "includeDeleted",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "containerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all Container Versions of a GTM Container"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bde97885-f35f-4044-b6f1-77fbcbbf091c"
            }
          ]
        }
      ]
    }
  ]
}