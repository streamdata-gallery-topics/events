---
swagger: "2.0"
info:
  title: Meetup OpenVenues
  description: Searches for public venues within a given geo space. To search for
    specific venues that your group has used, use the [Venues](/meetup_api/docs/2/venues)
    method
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
  /2/open_venues:
    get:
      summary: OpenVenues
      description: Searches for public venues within a given geo space
      operationId: venues
      parameters:
      - in: query
        name: api_version
        description: "2"
        type: string
      - in: query
        name: city
        description: A valid city
        type: string
      - in: query
        name: country
        description: A valid country code
        type: string
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: group_urlname
        description: Returns venues with location relative to the group associated
          with this urlname
        type: string
      - in: query
        name: lat
        description: A valid latitude, limits the returned venues to those within
          radius miles
        type: string
      - in: query
        name: lon
        description: A valid longitude, limits the returned venues to those within
          radius miles
        type: string
      - in: query
        name: radius
        description: Radius, in miles for geographic requests, default 25
        type: string
      - in: query
        name: since_count
        description: Request that some number of recent messages be sent immediately,
          if available
        type: string
      - in: query
        name: since_mtime
        description: Return recent open venues with an mtime greater then the supplied
          time, in milliseconds since the epoch
        type: string
      - in: query
        name: state
        description: For the US, a valid 2 character state code
        type: string
      - in: query
        name: text
        description: Venues that contain the given term or terms somewhere in their
          content
        type: string
      - in: query
        name: trickle
        description: When supplied with a request, the Meetup API will push your client
          the entire Meetup database of public venues in batches of 512
        type: string
      - in: query
        name: zip
        description: A valid US zip code, limits the returned venues to those within
          radius miles
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
      - photos
definitions: []
x-collection-name: Meetup
x-streamrank:
  polling_total_time_average: "0.47"
  polling_size_download_average: "208293.58"
  streaming_total_time_average: "0.26"
  streaming_size_download_average: "104828.22"
  change_yes: "50"
  change_no: "1811"
  time_percentage: "44"
  size_percentage: "50"
  change_percentage: "3"
  last_run: "2018-05-12"
  days_run: "8"
  minute_run: "0"
---