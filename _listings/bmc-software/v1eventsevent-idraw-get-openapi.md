---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Get raw events
  version: 1.0.0
  description: Returns all of the event occurrences (raw events) for the specified
    event.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/events:
    post:
      summary: Create event
      description: Creates an event. Every event occurrence is persisted to the database
        as a RawEvent. Based on the EventFingerprint, a new Event will be created
        or an existing one will be de-duplicated.
      operationId: create-event
      x-api-path-slug: v1events-post
      responses:
        200:
          description: OK
      tags:
      - Events
    get:
      summary: List events
      description: Searches for events in the specified organization.
      operationId: list-events
      x-api-path-slug: v1events-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/raw:
    get:
      summary: List raw events
      description: Queries all event occurrences (raw events) for the specified organization.
      operationId: list-raw-events
      x-api-path-slug: v1eventsraw-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/:event_id:
    get:
      summary: Get event
      description: Returns the event with the specified event id from the database.
      operationId: get-event
      x-api-path-slug: v1eventsevent-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/:event_id/raw:
    get:
      summary: Get raw events
      description: Returns all of the event occurrences (raw events) for the specified
        event.
      operationId: get-raw-events
      x-api-path-slug: v1eventsevent-idraw-get
      responses:
        200:
          description: OK
      tags:
      - Events
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