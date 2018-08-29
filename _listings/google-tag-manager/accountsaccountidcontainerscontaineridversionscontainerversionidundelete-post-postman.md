{
  "info": {
    "name": "Google Tag Manager API Undelete Container Version",
    "_postman_id": "ad6c4fae-9cca-4144-945d-08c80b839e9e",
    "description": "Undeletes a Container Version.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "containers",
      "item": [
        {
          "id": "050e4507-2f16-44e3-8f59-b2059093ba8c",
          "name": "tagmanager.accounts.containers.versions.undelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tagmanager",
                "v1",
                "accounts/:accountId/containers/:containerId/versions/:containerVersionId/undelete"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Undeletes a Container Version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a56bbe8c-5bb5-49ef-8249-150d0e13e9f1"
            }
          ]
        }
      ]
    }
  ]
}