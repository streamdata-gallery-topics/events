---
swagger: "2.0"
info:
  title: Meetup Close Rsvps
  description: Closes rsvps for an event
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:urlname/events/:event_id/rsvps/close:
    post:
      summary: Close Rsvps
      description: Closes rsvps for an event
      operationId: events
      responses:
        200:
          description: OK
      tags:
      - events
      - rsvp
definitions: []
x-collection-name: Meetup
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