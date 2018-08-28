{
  "info": {
    "name": "GIGANDCROWD Get Place Placeid Related",
    "_postman_id": "46bd56c4-159a-42f9-a920-129b509d48a2",
    "description": "Get place placeid related.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gigme",
      "item": [
        {
          "id": "ad5d6d54-231a-4435-98e3-ab94d954d326",
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
              "id": "7061aa5b-15ae-4be6-82ae-deecf596f78f"
            }
          ]
        },
        {
          "id": "09c7feef-3987-4821-9ea4-a78299fc9164",
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
              "id": "ed549dc1-e435-4af8-822c-f77f9daaf986"
            }
          ]
        }
      ]
    },
    {
      "name": "Place",
      "item": [
        {
          "id": "e1cf5f54-1bdf-47c8-b795-c4ac0fb400e5",
          "name": "getApiV1PlacePlaceRelated",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/place/:placeId/related"
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
            "description": "Get place placeid related."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a2a5469-1ab6-49e2-b551-49b6b0ed6d75"
            }
          ]
        }
      ]
    }
  ]
}