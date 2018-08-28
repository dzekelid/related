{
  "info": {
    "name": "GIGANDCROWD Get Gigme Place Placeid Related",
    "_postman_id": "d116d202-6c47-4114-8b3e-4438bfd62be6",
    "description": "Get gigme place placeid related.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gigme",
      "item": [
        {
          "id": "1f1268f9-7187-488e-aa99-94fca4de495e",
          "name": "getApiV1GigmeEventEventRelated",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/gigme/event/:eventId/related"
              ],
              "variable": [
                {
                  "id": "eventId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Get gigme event eventid related."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "990be81c-da4b-4c9c-bd55-cce3ffadcb20"
            }
          ]
        },
        {
          "id": "ac9a7026-99f6-4c56-92e5-18680fa05d61",
          "name": "getApiV1GigmePlacePlaceRelated",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/gigme/place/:placeId/related"
              ],
              "variable": [
                {
                  "id": "placeId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Get gigme place placeid related."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23f02e17-ae03-4f93-85fa-2b034a3ae105"
            }
          ]
        }
      ]
    }
  ]
}