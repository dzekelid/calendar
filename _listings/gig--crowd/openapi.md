---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/request/art/calendar:
    get:
      summary: Get Request Art Calendar
      description: Get request art calendar.
      operationId: getApiV1RequestArtCalendar
      x-api-path-slug: apiv1requestartcalendar-get
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: request.from
      - in: query
        name: request.to
      responses:
        200:
          description: OK
      tags:
      - Request
      - Art
      - Calendar
---