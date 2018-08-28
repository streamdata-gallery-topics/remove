---
swagger: "2.0"
x-collection-name: AWS Lambda
x-complete: 0
info:
  title: AWS Lambda API Delete Event Source Mapping
  version: 1.0.0
  description: Removes an event source mapping.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteEventSourceMapping:
    get:
      summary: Delete Event Source Mapping
      description: Removes an event source mapping.
      operationId: deleteEventSourceMapping
      x-api-path-slug: actiondeleteeventsourcemapping-get
      parameters:
      - in: query
        name: UUID
        description: The event source mapping ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Sources
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