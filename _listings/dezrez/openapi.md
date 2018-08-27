swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/sync/calendarsetup/{personId}:
    get:
      summary: Initially Setup the Calendar, create Rezi Calendar, copy upto 16 Days
        prior into calendar, create a subscription channel for the callback
      description: Initially setup the calendar, create rezi calendar, copy upto 16
        days prior into calendar, create a subscription channel for the callback.
      operationId: Sync_CalendarBypersonId
      x-api-path-slug: apisynccalendarsetuppersonid-get
      parameters:
      - in: path
        name: personId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Initially
      - Setup
      - Calendar
      - ""
      - Create
      - Rezi
      - Calendar
      - ""
      - Copy
      - Upto
      - "16"
      - Days
      - Prior
      - Into
      - Calendar
      - ""
      - Create
      - Subscription
      - Channelthe
      - Callback
  /api/sync/calendarsyncoauthurl/{personId}:
    get:
      summary: Get the oauth url for the calendar sync service
      description: Get the oauth url for the calendar sync service.
      operationId: Sync_CalendarSyncOauthUrlBypersonId
      x-api-path-slug: apisynccalendarsyncoauthurlpersonid-get
      parameters:
      - in: path
        name: personId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Urlthe
      - Calendar
      - Sync
      - Service
  /api/sync/calendarsyncenabled:
    get:
      summary: "check if the calendar sync is enabled for this user\r\nthis could
        be used to enabled/disable the calendar setup button"
      description: "Check if the calendar sync is enabled for this user\r\nthis could
        be used to enabled/disable the calendar setup button."
      operationId: Sync_CalendarSyncEnabled
      x-api-path-slug: apisynccalendarsyncenabled-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Check
      - If
      - Calendar
      - Sync
      - Is
      - Enabledthis
      - "User\r\nThis"
      - Could
      - Be
      - Used
      - To
      - Enabled
      - Disable
      - Calendar
      - Setup
      - Button
  /api/sync/cronofycallback/{negotiatorId}/{uniqueIdentifier}:
    post:
      summary: Forces a call to get updates from Cronofy for the rezi calendar
      description: Forces a call to get updates from cronofy for the rezi calendar.
      operationId: Sync_CronofyCallbackBynegotiatorIdByuniqueIdentifierBycalendarSyncResyncDataContract
      x-api-path-slug: apisynccronofycallbacknegotiatoriduniqueidentifier-post
      parameters:
      - in: body
        name: calendarSyncResyncDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: negotiatorId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: uniqueIdentifier
      responses:
        200:
          description: OK
      tags:
      - Forces
      - Call
      - To
      - Get
      - Updates
      - From
      - Cronofythe
      - Rezi
      - Calendar
  /api/sync/deletecalendar:
    delete:
      summary: Forces a call to get updates from Cronofy for the rezi calendar
      description: Forces a call to get updates from cronofy for the rezi calendar.
      operationId: Sync_DeleteCalendar
      x-api-path-slug: apisyncdeletecalendar-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Forces
      - Call
      - To
      - Get
      - Updates
      - From
      - Cronofythe
      - Rezi
      - Calendar