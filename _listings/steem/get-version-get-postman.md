{
  "info": {
    "name": "Steem get version of Steem",
    "_postman_id": "104c039a-d082-42f4-87f2-ac85ddb7134d",
    "description": "Returns version information of connected Steem node/websocket.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "34354b08-367f-400e-9632-e2173e3305e9",
          "name": "returns-version-information-of-connected-steem-nodewebsocket",
          "request": {
            "url": "http://api.steemjs.com/get_version",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns version information of connected Steem node/websocket."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "194bfb20-deb3-408f-b214-fe3ba222527f"
            }
          ]
        }
      ]
    }
  ]
}