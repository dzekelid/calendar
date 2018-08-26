---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Update Calendar
  description: Update calendar Update the properties of calendar object.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/calendars/{id}:
    delete:
      summary: Delete Calendar
      description: |-
        Delete calendar
        Delete a calendar other than the default calendar.
      operationId: DeleteCalendar
      x-api-path-slug: mecalendarsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    get:
      summary: Get Calendar
      description: |-
        Get calendar
        Retrieve the properties and relationships of calendar object.
      operationId: GetCalendar
      x-api-path-slug: mecalendarsid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    patch:
      summary: Update Calendar
      description: Update calendar Update the properties of calendar object.
      operationId: UpdateCalendar
      x-api-path-slug: mecalendarsid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /users/{id | userPrincipalName}/calendars/{id}:
    delete:
      summary: Delete Calendar
      description: |-
        Delete calendar
        Delete a calendar other than the default calendar.
      operationId: DeleteCalendar
      x-api-path-slug: usersid--userprincipalnamecalendarsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    get:
      summary: Get Calendar
      description: |-
        Get calendar
        Retrieve the properties and relationships of calendar object.
      operationId: GetCalendar
      x-api-path-slug: usersid--userprincipalnamecalendarsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    patch:
      summary: Update Calendar
      description: Update calendar Update the properties of calendar object.
      operationId: UpdateCalendar
      x-api-path-slug: usersid--userprincipalnamecalendarsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /me/calendarGroup/calendars/{id}:
    delete:
      summary: Delete Calendar
      description: |-
        Delete calendar
        Delete a calendar other than the default calendar.
      operationId: DeleteCalendar
      x-api-path-slug: mecalendargroupcalendarsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    get:
      summary: Get Calendar
      description: |-
        Get calendar
        Retrieve the properties and relationships of calendar object.
      operationId: GetCalendar
      x-api-path-slug: mecalendargroupcalendarsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    patch:
      summary: Update Calendar
      description: Update calendar Update the properties of calendar object.
      operationId: UpdateCalendar
      x-api-path-slug: mecalendargroupcalendarsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /users/{id | userPrincipalName}/calendarGroup/calendars/{id}:
    delete:
      summary: Delete Calendar
      description: |-
        Delete calendar
        Delete a calendar other than the default calendar.
      operationId: DeleteCalendar
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    get:
      summary: Get Calendar
      description: |-
        Get calendar
        Retrieve the properties and relationships of calendar object.
      operationId: GetCalendar
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    patch:
      summary: Update Calendar
      description: Update calendar Update the properties of calendar object.
      operationId: UpdateCalendar
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /me/calendarGroups/{id}/calendars/{id}:
    delete:
      summary: Delete Calendar
      description: |-
        Delete calendar
        Delete a calendar other than the default calendar.
      operationId: DeleteCalendar
      x-api-path-slug: mecalendargroupsidcalendarsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    get:
      summary: Get Calendar
      description: |-
        Get calendar
        Retrieve the properties and relationships of calendar object.
      operationId: GetCalendar
      x-api-path-slug: mecalendargroupsidcalendarsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}:
    delete:
      summary: Delete Calendar
      description: |-
        Delete calendar
        Delete a calendar other than the default calendar.
      operationId: DeleteCalendar
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    get:
      summary: Get Calendar
      description: |-
        Get calendar
        Retrieve the properties and relationships of calendar object.
      operationId: GetCalendar
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /me/calendar:
    get:
      summary: Get Calendar
      description: |-
        Get calendar
        Retrieve the properties and relationships of calendar object.
      operationId: GetCalendar
      x-api-path-slug: mecalendar-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    patch:
      summary: Update Calendar
      description: Update calendar Update the properties of calendar object.
      operationId: UpdateCalendar
      x-api-path-slug: mecalendar-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /users/{id | userPrincipalName}/calendar:
    get:
      summary: Get Calendar
      description: |-
        Get calendar
        Retrieve the properties and relationships of calendar object.
      operationId: GetCalendar
      x-api-path-slug: usersid--userprincipalnamecalendar-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    patch:
      summary: Update Calendar
      description: Update calendar Update the properties of calendar object.
      operationId: UpdateCalendar
      x-api-path-slug: usersid--userprincipalnamecalendar-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /groups/{id}/calendar:
    get:
      summary: Get Calendar
      description: |-
        Get calendar
        Retrieve the properties and relationships of calendar object.
      operationId: GetCalendar
      x-api-path-slug: groupsidcalendar-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
    patch:
      summary: Update Calendar
      description: Update calendar Update the properties of calendar object.
      operationId: UpdateCalendar
      x-api-path-slug: groupsidcalendar-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /me/calendar/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: mecalendarcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /users/{id | userPrincipalName}/calendar/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: usersid--userprincipalnamecalendarcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /groups/{id}/calendar/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: groupsidcalendarcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /me/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: mecalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /users/{id | userPrincipalName}/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: usersid--userprincipalnamecalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /me/calendarGroup/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: mecalendargroupcalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /me/calendarGroups/{id}/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: mecalendargroupsidcalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
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