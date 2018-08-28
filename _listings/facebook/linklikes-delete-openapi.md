---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Delete Link Likes
  description: Unlikes this link.
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{application}/links:
    get:
      summary: Get Application Links
      description: The application's posted links.
      operationId: getApplicationLinks
      x-api-path-slug: applicationlinks-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Links
    post:
      summary: Post Application Links
      description: Posts a link on the application's profile page
      operationId: postApplicationLinks
      x-api-path-slug: applicationlinks-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: link
        description: Link URL
      - in: query
        name: message
        description: Link message
      responses:
        200:
          description: OK
      tags:
      - Application
      - Links
  /{page}/links:
    get:
      summary: Get Page Links
      description: The page's posted links
      operationId: getPageLinks
      x-api-path-slug: pagelinks-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Links
    post:
      summary: Post Page Links
      description: Posts a link on the page
      operationId: postPageLinks
      x-api-path-slug: pagelinks-post
      parameters:
      - in: query
        name: link
        description: Link URL
      - in: query
        name: message
        description: Link message
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Links
  /{user}/links:
    get:
      summary: Get User Links
      description: The user's posted links.
      operationId: getUserLinks
      x-api-path-slug: userlinks-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Links
    post:
      summary: Post User Links
      description: Posts a link on the user's profile page
      operationId: postUserLinks
      x-api-path-slug: userlinks-post
      parameters:
      - in: query
        name: link
        description: Link URL
      - in: query
        name: message
        description: Link message
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Links
  /{link}:
    get:
      summary: Get Link
      description: A link shared on a user's wall
      operationId: getLink
      x-api-path-slug: link-get
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
  /{link}/comments:
    get:
      summary: Get Link Comments
      description: All of the comments on this link.
      operationId: getLinkComments
      x-api-path-slug: linkcomments-get
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
      - Comments
    post:
      summary: Post Link Comments
      description: Posts a comment to this link.
      operationId: postLinkComments
      x-api-path-slug: linkcomments-post
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      - in: query
        name: message
        description: Comment text
      responses:
        200:
          description: OK
      tags:
      - Link
      - Comments
  /{link}/likes:
    get:
      summary: Get Link Likes
      description: Users who like this link.
      operationId: getLinkLikes
      x-api-path-slug: linklikes-get
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
      - Likes
    post:
      summary: Post Link Likes
      description: Likes this link.
      operationId: postLinkLikes
      x-api-path-slug: linklikes-post
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
      - Likes
    delete:
      summary: Delete Link Likes
      description: Unlikes this link.
      operationId: deleteLinkLikes
      x-api-path-slug: linklikes-delete
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
      - Likes
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