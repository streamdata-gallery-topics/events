swagger: "2.0"
x-collection-name: TigerText
x-complete: 1
info:
  title: TigerConnect User API
  description: the-user-system-for-tigerconnect-messaging-platform-
  termsOfService: http://www.tigertext.com/developer-terms-of-use
  contact:
    name: TigerText
    url: http://www.tigertext.com/supportform/
    email: info@tigertext.com
  version: v2
host: developer.tigertext.me
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/:
    delete:
      summary: Drop the events connections.
      description: Drop the events connections.
      operationId: dropConnect
      x-api-path-slug: events-delete
      responses:
        200:
          description: OK
      tags:
      - Events
    get:
      summary: Opens a SSE event stream.
      description: Opens a SSE event stream. The various Event Types are listed below.
      operationId: createEvents
      x-api-path-slug: events-get
      responses:
        200:
          description: OK
      tags:
      - Events