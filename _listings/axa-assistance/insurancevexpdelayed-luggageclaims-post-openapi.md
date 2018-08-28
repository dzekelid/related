---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Requests to create a claim related to a delayed luggage.
  description: Requests to create a claim related to a delayed luggage.
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /assistance/v1/home/water_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the information related to each the policy holder of the water
        damage declaration
      description: Gets the information related to each the policy holder of the water
        damage declaration
      operationId: getAssistanceV1HomeWater_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homewater-damagedeclarationsdeclaration-idpolicy-holders-get
      parameters:
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - information
      - related
      - to
      - each
      - the
      - policy
      - holder
      - of
      - the
      - water
      - damage
      - Declarations
  /insurance/vexp/appliance/claims:
    post:
      summary: Requests to create a claim related to an appliance.
      description: Requests to create a claim related to an appliance.
      operationId: postInsuranceVexpApplianceClaims
      x-api-path-slug: insurancevexpapplianceclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - toappliance.
  /insurance/vexp/car_rental/claims:
    post:
      summary: Requests to create a claim related to a car rental.
      description: Requests to create a claim related to a car rental.
      operationId: postInsuranceVexpCar_rentalClaims
      x-api-path-slug: insurancevexpcar-rentalclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - tocar
      - rental.
  /insurance/vexp/corporate_liability/claims:
    post:
      summary: Requests to create a claim related to a corporate liability.
      description: Requests to create a claim related to a corporate liability.
      operationId: postInsuranceVexpCorporate_liabilityClaims
      x-api-path-slug: insurancevexpcorporate-liabilityclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - tocorporate
      - liability.
  /insurance/vexp/delayed_luggage/claims:
    post:
      summary: Requests to create a claim related to a delayed luggage.
      description: Requests to create a claim related to a delayed luggage.
      operationId: postInsuranceVexpDelayed_luggageClaims
      x-api-path-slug: insurancevexpdelayed-luggageclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - todelayed
      - luggage.
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