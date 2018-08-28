---
swagger: "2.0"
x-collection-name: BigOven
x-complete: 0
info:
  title: Big Oven Get recipes related to the given recipeId
  description: Get recipes related to the given recipeid.
  termsOfService: Please see our [terms of service](http://api2.bigoven.com/web/documentation/termsofuse
  version: partner
host: api2.bigoven.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /recipe/{recipeId}/related:
    get:
      summary: Get recipes related to the given recipeId
      description: Get recipes related to the given recipeid.
      operationId: Recipe_Related
      x-api-path-slug: reciperecipeidrelated-get
      parameters:
      - in: query
        name: pg
      - in: path
        name: recipeId
      - in: query
        name: rpp
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
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