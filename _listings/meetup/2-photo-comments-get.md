---
swagger: "2.0"
info:
  title: Meetup Photo Comments v2
  description: This method returns comments on meetup photos. To post messages, see
    the corresponding write method
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
  /2/photo_comments:
    get:
      summary: Photo Comments v2
      description: This method returns comments on meetup photos
      operationId: photos
      parameters:
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: member_id
        description: Return comments for the given member_ids, separated by commas
        type: string
      - in: query
        name: photo_id
        description: Return comments on these photos, separated by commas
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
      - profile
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