{
  "info": {
    "name": "Google Tag Manager API Restore Container Version",
    "_postman_id": "375b8783-d819-4ac2-8ccc-97b9b1c7ccf8",
    "description": "Restores a Container Version. This will overwrite the container's current configuration (including its variables, triggers and tags). The operation will not have any effect on the version that is being served (i.e. the published version).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "containers",
      "item": [
        {
          "id": "bfa379fe-bee3-436f-9213-a51a6d55e46f",
          "name": "tagmanager.accounts.containers.versions.restore",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tagmanager",
                "v1",
                "accounts/:accountId/containers/:containerId/versions/:containerVersionId/restore"
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
            "description": "Restores a Container Version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ded25a02-1e70-4ea0-98ed-dc40d4b641c3"
            }
          ]
        }
      ]
    }
  ]
}