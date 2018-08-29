{
  "info": {
    "name": "Google Tag Manager API Get Container Version",
    "_postman_id": "e5bf9c10-e8f5-4995-9669-0ebfffa02f35",
    "description": "Gets a Container Version.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "containers",
      "item": [
        {
          "id": "095a7d6f-4227-41df-acd1-61b5104c546d",
          "name": "tagmanager.accounts.containers.versions.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tagmanager",
                "v1",
                "accounts/:accountId/containers/:containerId/versions/:containerVersionId"
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
                },
                {
                  "id": "containerVersionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a Container Version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b8a2d8c-883f-41d1-9f94-e52891cf6e77"
            }
          ]
        }
      ]
    }
  ]
}