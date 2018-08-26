---
swagger: "2.0"
x-collection-name: Google Calendar
x-complete: 1
info:
  title: Google Calendar
  description: manipulates-events-and-other-calendar-data-
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
    get:
      summary: Get Calendar
      description: Returns metadata for a calendar.
      operationId: calendar.calendars.get
      x-api-path-slug: calendarscalendarid-get
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar
    patch:
      summary: Update Calendar
      description: Updates metadata for a calendar. This method supports patch semantics.
      operationId: calendar.calendars.patch
      x-api-path-slug: calendarscalendarid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar
    put:
      summary: Update Calendar
      description: Updates metadata for a calendar.
      operationId: calendar.calendars.update
      x-api-path-slug: calendarscalendarid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /calendars/{calendarId}/clear:
    post:
      summary: Clear Primary Calendar
      description: Clears a primary calendar. This operation deletes all events associated
        with the primary calendar of an account.
      operationId: calendar.calendars.clear
      x-api-path-slug: calendarscalendaridclear-post
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar
---