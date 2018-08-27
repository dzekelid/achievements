---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 0
info:
  title: Google Play Set Steps for Achievements
  version: 1.0.0
  description: Sets the steps for the currently authenticated player towards unlocking
    an achievement. If the steps parameter is less than the current number of steps
    that the player already gained for the achievement, the achievement is not modified.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /achievements:
    get:
      summary: Get Achievements
      description: Lists all the achievement definitions for your application.
      operationId: games.achievementDefinitions.list
      x-api-path-slug: achievements-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of achievement resources to return in the
          response, used for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Achievement
  /achievements/updateMultiple:
    post:
      summary: Update Multiple Achievements
      description: Updates multiple achievements for the currently authenticated player.
      operationId: games.achievements.updateMultiple
      x-api-path-slug: achievementsupdatemultiple-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Achievement
  /achievements/{achievementId}/setStepsAtLeast:
    post:
      summary: Set Steps for Achievements
      description: Sets the steps for the currently authenticated player towards unlocking
        an achievement. If the steps parameter is less than the current number of
        steps that the player already gained for the achievement, the achievement
        is not modified.
      operationId: games.achievements.setStepsAtLeast
      x-api-path-slug: achievementsachievementidsetstepsatleast-post
      parameters:
      - in: path
        name: achievementId
        description: The ID of the achievement used by this method
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: steps
        description: The minimum value to set the steps to
      responses:
        200:
          description: OK
      tags:
      - Achievement
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