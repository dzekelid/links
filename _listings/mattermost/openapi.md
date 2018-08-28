swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{file_id}/link:
    get:
      summary: Get a public file link
      description: Gets a public link for a file that can be accessed without logging
        into Mattermost.
      operationId: gets-a-public-link-for-a-file-that-can-be-accessed-without-logging-into-mattermost
      x-api-path-slug: filesfile-idlink-get
      parameters:
      - in: path
        name: file_id
        description: The ID of the file to get a link for
      responses:
        200:
          description: OK
      tags:
      - Public
      - File
      - Link