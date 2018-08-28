---
swagger: "2.0"
x-collection-name: Hacker News
x-complete: 0
info:
  title: Hacker News Get the current largest item id
  description: Get the current largest item id
  version: 1.0.0
host: hacker-news.firebaseio.com
basePath: /v0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /updates.json:
    get:
      summary: Get the changed items and profiles
      description: Get the changed items and profiles
      operationId: get
      x-api-path-slug: updates-json-get
      responses:
        200:
          description: Successful response
      tags:
      - Links
      - Stories
      - Updates
  /topstories.json:
    get:
      summary: Returns the current top 100 stories.
      description: Returns the current top 100 stories.
      operationId: get_top_stories
      x-api-path-slug: topstories-json-get
      responses:
        200:
          description: Successful response
      tags:
      - Links
      - Stories
      - Top
  /user/{id}.json:
    get:
      summary: Users are identified by case-sensitive ids
      description: Users are identified by case-sensitive ids
      operationId: get_user
      x-api-path-slug: userid-json-get
      parameters:
      - in: path
        name: id
        description: User ID
      responses:
        200:
          description: Successful response
      tags:
      - Links
      - Stories
  /maxitem.json:
    get:
      summary: Get the current largest item id
      description: Get the current largest item id
      operationId: get_max_item
      x-api-path-slug: maxitem-json-get
      responses:
        200:
          description: Successful response
      tags:
      - Links
      - Stories
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