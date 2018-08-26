{
  "info": {
    "name": "Microsoft Office 365 Get Calendar",
    "_postman_id": "b35866c6-9e59-4f67-8c66-c5b79c7ec93d",
    "description": "Retrieve information about the default calendar by using the...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Allservices",
      "item": [
        {
          "id": "0362364a-0d70-423e-affc-60a461bcfe77",
          "name": "getAllservices",
          "request": {
            "url": "http://outlook.office365.com/ews/odata/Me/AllServices",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all services."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ff62353-bee1-4690-b4ae-aa88b099bf72"
            }
          ]
        }
      ]
    },
    {
      "name": "Calendar",
      "item": [
        {
          "id": "3a1cd8b9-4e1e-438e-9734-4bc604d5b47f",
          "name": "getCalendar",
          "request": {
            "url": "http://outlook.office365.com/ews/odata/Me/Calendar",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve information about the default calendar by using the..."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2dd663b0-bb89-46fa-81ee-1eea9df0eb63"
            }
          ]
        }
      ]
    }
  ]
}