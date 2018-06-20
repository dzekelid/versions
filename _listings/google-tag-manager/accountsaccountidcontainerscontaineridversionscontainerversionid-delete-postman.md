{
  "info": {
    "name": "Google Tag Manager API Delete Container Version",
    "_postman_id": "424dd94e-47a0-42cf-86df-b24a3e5d96b9",
    "description": "Deletes a Container Version.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "containers",
      "item": [
        {
          "id": "0f312c21-5fc7-41da-a32f-b3300a365168",
          "name": "tagmanager.accounts.containers.versions.delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Container Version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d021b13-6bb3-4c89-b05d-e08a2859d2e6"
            }
          ]
        }
      ]
    }
  ]
}