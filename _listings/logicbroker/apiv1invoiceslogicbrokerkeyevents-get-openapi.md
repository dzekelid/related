---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Retrieve related events
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Shipments/{LogicbrokerKey}/Events:
    get:
      summary: Retrieve related events
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetActivityEvent
      x-api-path-slug: apiv1shipmentslogicbrokerkeyevents-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Related
      - Events
  /api/v1/Orders/{LogicbrokerKey}/Events:
    get:
      summary: Retrieve related events
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetActivityEvent
      x-api-path-slug: apiv1orderslogicbrokerkeyevents-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Related
      - Events
  /api/v1/Invoices/{LogicbrokerKey}/Events:
    get:
      summary: Retrieve related events
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Invoice_GetActivityEvent
      x-api-path-slug: apiv1invoiceslogicbrokerkeyevents-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Related
      - Events
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