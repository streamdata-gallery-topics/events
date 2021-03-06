---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Calendar Get Events For Tomorrow
  description: Get all the events released tomorrow.
  version: 1.0.0
host: www.xignite.com
basePath: xCalendar.json/XigniteCalendar
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetEventsForNextNumberOfDays:
    get:
      summary: Get Events For Next Number Of Days
      description: Get events for the next number of days into the future.
      operationId: postGeteventsfornextnumberofdays
      x-api-path-slug: geteventsfornextnumberofdays-get
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
      - Events
      - Next
      - Number
      - Days
  /GetEventsForWeek:
    get:
      summary: Get Events For Week
      description: Get all the events released during the week specified. Weeks are
        Monday - Sunday.
      operationId: postGeteventsforweek
      x-api-path-slug: geteventsforweek-get
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
      - Events
      - Week
  /GetEventsByCountryCode:
    get:
      summary: Get Events By Country Code
      description: Get events based on the country code and optionally within a specified
        released range.
      operationId: postGeteventsbycountrycode
      x-api-path-slug: geteventsbycountrycode-get
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
      - Events
      - Country
      - Code
  /GetMostRecentEventsByEventCode:
    get:
      summary: Get Most Recent Events By Event Code
      description: Get the most recent events based on the event code and count.
      operationId: postGetmostrecenteventsbyeventcode
      x-api-path-slug: getmostrecenteventsbyeventcode-get
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
      - Most
      - Recent
      - Events
      - Event
      - Code
  /GetEventsByEventCode:
    get:
      summary: Get Events By Event Code
      description: Get events based on the event code and optionally within a specified
        released range.
      operationId: postGeteventsbyeventcode
      x-api-path-slug: geteventsbyeventcode-get
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
      - Events
      - Event
      - Code
  /GetEventsByEventName:
    get:
      summary: Get Events By Event Name
      description: Get events based on the event name and optionally within a specified
        released range.
      operationId: postGeteventsbyeventname
      x-api-path-slug: geteventsbyeventname-get
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
      - Events
      - Event
      - Name
  /GetEventsForDate:
    get:
      summary: Get Events For Date
      description: Get events for the specified date.
      operationId: postGeteventsfordate
      x-api-path-slug: geteventsfordate-get
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
      - Events
      - Date
  /GetEventsForMonth:
    get:
      summary: Get Events For Month
      description: Get events for the specified date.
      operationId: postGeteventsformonth
      x-api-path-slug: geteventsformonth-get
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
      - Events
      - Month
  /GetEventsForRange:
    get:
      summary: Get Events For Range
      description: Get events for the specified range.
      operationId: postGeteventsforrange
      x-api-path-slug: geteventsforrange-get
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
      - Events
      - Range
  /GetEventsForRangeLength:
    get:
      summary: Get Events For Range Length
      description: Get events for the date specified and next number of days past
        it.
      operationId: postGeteventsforrangelength
      x-api-path-slug: geteventsforrangelength-get
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
      - Events
      - Range
      - Length
  /GetEventsForToday:
    get:
      summary: Get Events For Today
      description: Get all the events released today.
      operationId: postGeteventsfortoday
      x-api-path-slug: geteventsfortoday-get
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
      - Events
      - Today
  /GetEventsForTomorrow:
    get:
      summary: Get Events For Tomorrow
      description: Get all the events released tomorrow.
      operationId: postGeteventsfortomorrow
      x-api-path-slug: geteventsfortomorrow-get
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
      - Events
      - Tomorrow
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