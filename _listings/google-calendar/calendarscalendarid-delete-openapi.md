---
swagger: "2.0"
x-collection-name: Google Calendar
x-complete: 0
info:
  title: Google Calendar CreaDeletete Calendar
  description: Deletes a secondary calendar. Use calendars.clear for clearing all
    events on primary calendars.
  contact:
    name: Google
    url: https://google.com
  version: v3/
host: www.googleapis.com
basePath: /calendar/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calendars:
    post:
      summary: Create Calendar
      description: Creates a secondary calendar.
      operationId: calendar.calendars.insert
      x-api-path-slug: calendars-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /calendars/{calendarId}:
    delete:
      summary: CreaDeletete Calendar
      description: Deletes a secondary calendar. Use calendars.clear for clearing
        all events on primary calendars.
      operationId: calendar.calendars.delete
      x-api-path-slug: calendarscalendarid-delete
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar
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