swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /articles/{slug}/related-listings:
    get:
      summary: Get Articles Slug Related Listings
      description: Find listings related to an article
      operationId: getArticlesSlugRelatedListings
      x-api-path-slug: articlesslugrelatedlistings-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Articles
      - Slug
      - Related-listings