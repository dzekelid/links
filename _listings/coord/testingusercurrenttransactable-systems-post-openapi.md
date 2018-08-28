---
swagger: "2.0"
x-collection-name: Coord
x-complete: 0
info:
  title: Coord Users API Simulate account linking for testing
  description: |-
    Link a test user account to a system. This endpoint simulates the account linking flow
    outlined in `/user/current/link_account`. To link the test user's account with CitiBike,
    send:

    ```
    {
      "system_id": "CitiBike",
      "linked_account": true
    }
    ```

    On success, the response will be the same transactable system:
    ```
    {
      "system_id": "CitiBike",
      "linked_account": true
    }
    ```

    You can also unlink a system by setting `linked_account` to `false` instead. The full list
    of the user's current transactable systems can be found in the `transactable_systems` field
    when you call `GET /v1/users/user/current`.

    Not all systems require account linking to be transactable, and some systems require you to
    send additional information in order to connect to them. We will return a `400` if the user
    would not be able to link their account due to one of these reasons.

    ** Note that this method will not work for non-test users. **
  version: 1.0.0
host: api.coord.co
basePath: /v1/users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /testing/user/current/transactable_systems:
    post:
      summary: Simulate account linking for testing
      description: |-
        Link a test user account to a system. This endpoint simulates the account linking flow
        outlined in `/user/current/link_account`. To link the test user's account with CitiBike,
        send:

        ```
        {
          "system_id": "CitiBike",
          "linked_account": true
        }
        ```

        On success, the response will be the same transactable system:
        ```
        {
          "system_id": "CitiBike",
          "linked_account": true
        }
        ```

        You can also unlink a system by setting `linked_account` to `false` instead. The full list
        of the user's current transactable systems can be found in the `transactable_systems` field
        when you call `GET /v1/users/user/current`.

        Not all systems require account linking to be transactable, and some systems require you to
        send additional information in order to connect to them. We will return a `400` if the user
        would not be able to link their account due to one of these reasons.

        ** Note that this method will not work for non-test users. **
      operationId: test_link_user_account
      x-api-path-slug: testingusercurrenttransactable-systems-post
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: body
        name: system
        description: The system the user should be provisioned for
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Simulate
      - Account
      - Linkingtesting
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