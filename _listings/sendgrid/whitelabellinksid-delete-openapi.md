---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Delete Whitelabel Links
  description: |-
    **This endpoint allows you to delete a link whitelabel.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /whitelabel/links:
    get:
      summary: Get Whitelabel Links
      description: |-
        **This endpoint allows you to retrieve all link whitelabels.**

        Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

        For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
      operationId: whitelabel.links.get
      x-api-path-slug: whitelabellinks-get
      parameters:
      - in: query
        name: limit
        description: Limits the number of results returned per page
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Links
    post:
      summary: Add Whitelabel Links
      description: |-
        **This endpoint allows you to create a new link whitelabel.**

        Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

        For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
      operationId: whitelabel.links.post
      x-api-path-slug: whitelabellinks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: limit
        description: Number of domains to return
      - in: query
        name: No Name
      - in: query
        name: offset
        description: Paging offset
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Links
  /whitelabel/links/default:
    get:
      summary: Get Whitelabel Links Default
      description: |-
        **This endpoint allows you to retrieve the default link whitelabel.**

        Default link whitelabel is the actual link whitelabel to be used when sending messages. If there are multiple link whitelabels, the default is determined by the following order:
        <ul>
          <li>Validated link whitelabels marked as "default"</li>
          <li>Legacy link whitelabels (migrated from the whitelabel wizard)</li>
          <li>Default SendGrid link whitelabel (i.e. 100.ct.sendgrid.net)</li>
        </ul>

        Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

        For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
      operationId: whitelabel.links.default.get
      x-api-path-slug: whitelabellinksdefault-get
      parameters:
      - in: query
        name: domain
        description: The domain to match against when finding a corresponding link
          whitelabel
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Links
      - Default
  /whitelabel/links/subuser:
    delete:
      summary: Delete Whitelabel Links Subuser
      description: |-
        **This endpoint allows you to disassociate a link whitelabel from a subuser.**

        Link whitelables can be associated with subusers from the parent account. This functionality allows
        subusers to send mail using their parent's linke whitelabels. To associate a link whitelabel, the parent account
        must first create a whitelabel and validate it. The parent may then associate that whitelabel with a subuser via the API or the Subuser Management page in the user interface.

        Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

        For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
      operationId: whitelabel.links.subuser.delete
      x-api-path-slug: whitelabellinkssubuser-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: query
        name: username
        description: The username of the subuser account that you want to disassociate
          a link whitelabel from
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Links
      - Subuser
    get:
      summary: Get Whitelabel Links Subuser
      description: |-
        **This endpoint allows you to retrieve the associated link whitelabel for a subuser.**

        Link whitelables can be associated with subusers from the parent account. This functionality allows
        subusers to send mail using their parent's linke whitelabels. To associate a link whitelabel, the parent account
        must first create a whitelabel and validate it. The parent may then associate that whitelabel with a subuser via the API or the Subuser Management page in the user interface.

        Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

        For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
      operationId: whitelabel.links.subuser.get
      x-api-path-slug: whitelabellinkssubuser-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: username
        description: The username of the subuser to retrieve associated link whitelabels
          for
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Links
      - Subuser
  /whitelabel/links/{id}:
    delete:
      summary: Delete Whitelabel Links
      description: |-
        **This endpoint allows you to delete a link whitelabel.**

        Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

        For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
      operationId: whitelabel.links.id.delete
      x-api-path-slug: whitelabellinksid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Links
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