{
  "info": {
    "name": "Google Tag Manager API Publish Container Version",
    "_postman_id": "5d7942ac-4e97-495b-8ab6-8600af3fd400",
    "description": "Publishes a Container Version.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "containers",
      "item": [
        {
          "id": "cdfa7f64-d1ba-41d5-b769-e64c9721a657",
          "name": "tagmanager.accounts.containers.versions.publish",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tagmanager",
                "v1",
                "accounts/:accountId/containers/:containerId/versions/:containerVersionId/publish"
              ],
              "query": [
                {
                  "key": "fingerprint",
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
            "description": "Publishes a Container Version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58423419-da25-438a-8257-853e105ed32c"
            }
          ]
        }
      ]
    }
  ]
}