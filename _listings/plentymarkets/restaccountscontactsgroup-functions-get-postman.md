{
  "info": {
    "name": "Plentymarkets List all group function related data",
    "_postman_id": "e10dbf2f-a35a-45bf-960b-67b951a83651",
    "description": "Lists all data that is related to the contact group function contents.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "10a85d7d-0b03-4b92-a481-873b722dd81f",
          "name": "getRestAccountsContactsGroupFunctions",
          "request": {
            "url": "http://example.com/rest/accounts/contacts/group_functions",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists all data that is related to the contact group function contents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68bddd2e-69a9-4503-a0e8-4c5351b78aeb"
            }
          ]
        }
      ]
    }
  ]
}