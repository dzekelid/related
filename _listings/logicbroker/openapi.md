swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
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