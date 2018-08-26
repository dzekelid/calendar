{
  "info": {
    "name": "Microsoft Office 365 Delete Calendars Calendar",
    "_postman_id": "2118acf9-9e4f-441a-afd2-2c18ffed4659",
    "description": "Deleting a calendar is as simple as sending a DELETE request...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "calendars",
      "item": [
        {
          "id": "a637b497-d18f-47da-aa63-f684875edade",
          "name": "deleteCalendarsCalendar",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deleting a calendar is as simple as sending a DELETE request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87bf209d-a7a7-4581-84ee-e0b4d674e80b"
            }
          ]
        }
      ]
    }
  ]
}