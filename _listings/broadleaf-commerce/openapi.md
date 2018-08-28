swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /related-products:
    get:
      summary: Get Related Products
      description: Get related products.
      operationId: getRelatedProducts
      x-api-path-slug: relatedproducts-get
      parameters:
      - in: query
        name: categoryId
        description: categoryId
      - in: query
        name: categoryKey
        description: categoryKey
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      - in: query
        name: productId
        description: productId
      - in: query
        name: productKey
        description: productKey
      - in: query
        name: quantity
        description: quantity
      - in: query
        name: type
        description: type
      responses:
        200:
          description: OK
      tags:
      - Related
      - Products