---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Place Placeid Related
  version: 1.0.0
  description: Get place placeid related.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---