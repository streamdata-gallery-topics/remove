---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: Victor Ops Remove a user
  description: |-
    Remove a user from your organization

    This API may be called a maximum of 15 times per minute.
  version: 0.0.2
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-public/v1/team/{team}:
    delete:
      summary: Remove a team
      description: |-
        Remove a team from your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.delete
      x-api-path-slug: apipublicv1teamteam-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to be deleted
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
  /api-public/v1/team/{team}/members/{user}:
    delete:
      summary: Remove a team member
      description: |-
        Remove a team from your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.members.user.delete
      x-api-path-slug: apipublicv1teamteammembersuser-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to be deleted
      - in: path
        name: user
        description: The team member username
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
      - Members
      - User
  /api-public/v1/user/{user}:
    delete:
      summary: Remove a user
      description: |-
        Remove a user from your organization

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.delete
      x-api-path-slug: apipublicv1useruser-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user to be deleted
      responses:
        200:
          description: OK
      tags:
      - User
      - User
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