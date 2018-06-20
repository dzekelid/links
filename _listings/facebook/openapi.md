---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  description: connect-to-the-social-network-with-the-graph-api-
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
---