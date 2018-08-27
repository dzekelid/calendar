swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetIPOCalendar:
    get:
      summary: Get IPO Calendar
      description: Post getipocalendar
      operationId: GetIPOCalendar
      x-api-path-slug: getipocalendar-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - IPO
      - Calendar
  /GetIPOCalendarByExchange:
    get:
      summary: Get IPO Calendar By Exchange
      description: Post getipocalendarbyexchange
      operationId: GetIPOCalendarByExchange
      x-api-path-slug: getipocalendarbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - IPO
      - Calendar
      - Exchange