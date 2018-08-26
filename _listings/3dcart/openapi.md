---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 1
info:
  title: _3dCartWebAPI
  version: 1.0.0
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Products/{catalogid}/Related:
    get:
      summary: Get the related products from a specific Product
      description: Get the related products from a specific product.
      operationId: Products_GetAllProductRelated
      x-api-path-slug: 3dcartwebapiv1productscatalogidrelated-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Related
      - Products
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of related products from a specific Product
      description: Updates a collection of related products from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidrelated-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: relatedproducts
        description: A Json or XML object containing the new related products
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Related
      - Products
      - From
      - Specific
      - Product
    post:
      summary: Adds a new related product to the system
      description: Adds a new related product to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidrelated-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: relatedproduct
        description: A Json or XML object containing the new related product
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Related
      - Product
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Related/{relatedindexid}:
    put:
      summary: Updates a specific related product from a specific Product
      description: Updates a specific related product from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidrelatedrelatedindexid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: path
        name: relatedindexid
        description: RelatedIndexID
      - in: body
        name: relatedproduct
        description: A Json or XML object containing the new related products
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Related
      - Product
      - From
      - Specific
      - Product
---