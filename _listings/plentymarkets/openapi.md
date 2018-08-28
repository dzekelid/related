swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/group_functions:
    get:
      summary: List all group function related data
      description: Lists all data that is related to the contact group function contents.
      operationId: getRestAccountsContactsGroupFunctions
      x-api-path-slug: restaccountscontactsgroup-functions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Group
      - Function
      - Related
      - Data
  /rest/accounts/contacts/{contactId}/related_data:
    get:
      summary: Return all contact related data
      description: Returns all contact related data.
      operationId: getRestAccountsContactsContactRelatedData
      x-api-path-slug: restaccountscontactscontactidrelated-data-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Return
      - ""
      - Contact
      - Related
      - Data