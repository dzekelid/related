swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/gigme/event/{eventId}/related:
    get:
      summary: Get Gigme Event Eventid Related
      description: Get gigme event eventid related.
      operationId: getApiV1GigmeEventEventRelated
      x-api-path-slug: apiv1gigmeeventeventidrelated-get
      parameters:
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Eventid
      - Related
  /api/v1/gigme/place/{placeId}/related:
    get:
      summary: Get Gigme Place Placeid Related
      description: Get gigme place placeid related.
      operationId: getApiV1GigmePlacePlaceRelated
      x-api-path-slug: apiv1gigmeplaceplaceidrelated-get
      parameters:
      - in: path
        name: placeId
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Place
      - Placeid
      - Related
  /api/v1/place/{placeId}/related:
    get:
      summary: Get Place Placeid Related
      description: Get place placeid related.
      operationId: getApiV1PlacePlaceRelated
      x-api-path-slug: apiv1placeplaceidrelated-get
      parameters:
      - in: path
        name: placeId
      responses:
        200:
          description: OK
      tags:
      - Place
      - Placeid
      - Related