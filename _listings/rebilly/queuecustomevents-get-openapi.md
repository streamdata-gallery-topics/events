---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Retrieve a list of scheduled custom events
  description: Retrieve a list of scheduled custom events
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /custom-events:
    get:
      summary: Retrieve a list of custom events
      description: Retrieve a list of custom events
      operationId: retrieve-a-list-of-custom-events
      x-api-path-slug: customevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Custom
      - Events
  /events:
    get:
      summary: Retrieve a list of existing events
      description: ""
      operationId: ""
      x-api-path-slug: events-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Existing
      - Events
  /queue/custom-events:
    get:
      summary: Retrieve a list of scheduled custom events
      description: Retrieve a list of scheduled custom events
      operationId: retrieve-a-list-of-scheduled-custom-events
      x-api-path-slug: queuecustomevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Scheduled
      - Custom
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