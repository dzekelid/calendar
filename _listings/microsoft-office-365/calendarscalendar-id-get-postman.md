{
  "info": {
    "name": "Microsoft Office 365 Get Calendars Calendar",
    "_postman_id": "817d731a-a251-4c9f-9e46-e7635be08c93",
    "description": "You can also retrieve information about a specific calendar ...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "calendars",
      "item": [
        {
          "id": "b3ebaa50-075d-4aba-92cd-2f448aa877f5",
          "name": "getCalendarsCalendar",
          "request": {
            "url": {
              "protocol": "http",
              "host": "outlook.office365.com",
              "path": [
                "ews",
                "odata",
                "Me",
                "Calendars:calendar_id"
              ],
              "variable": [
                {
                  "id": "calendar_id",
                  "value": "calendar_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can also retrieve information about a specific calendar "
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d267a5c-1315-458e-a0df-bd1f7edf92d5"
            }
          ]
        }
      ]
    }
  ]
}