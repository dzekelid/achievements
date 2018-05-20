---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get User Achievements
  description: User Achievements
  termsOfService: https://www.facebook.com/policies/
  version: 1.0.0
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;user-id&#125;/achievements:
    get:
      summary: Get User Achievements
      description: User Achievements
      operationId: getUserAchievements
      x-api-path-slug: 123userid125achievements-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Achievements
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