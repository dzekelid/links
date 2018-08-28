---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Delete remote version links by version id
  description: Delete all remote version links for a given version ID.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/issue/{issueIdOrKey}/remotelink:
    get:
      summary: Get remote issue links
      description: Returns the remote issue links for the issue. This may be links
        to other Jira instances, web applications or web pages.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getRemoteIssueLinks_get
      x-api-path-slug: api2issueissueidorkeyremotelink-get
      parameters:
      - in: query
        name: globalId
        description: ID of the remote issue link to be returned
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to retrieve remote links for
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Issue
      - Links
  /api/2/version/remotelink:
    get:
      summary: Get remote version links
      description: Returns the remote version links for a given global ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getRemoteVersionLinks_get
      x-api-path-slug: api2versionremotelink-get
      parameters:
      - in: query
        name: globalId
        description: the global ID of the remote resource that is linked to the versions
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Links
  /api/2/version/{versionId}/remotelink:
    get:
      summary: Get remote version links by version id
      description: Returns the remote version links associated with the given version
        ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getRemoteVersionLinksByVersionId_get
      x-api-path-slug: api2versionversionidremotelink-get
      parameters:
      - in: path
        name: versionId
        description: a String containing the version ID
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Links
      - By
      - Version
      - Id
    delete:
      summary: Delete remote version links by version id
      description: Delete all remote version links for a given version ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.deleteRemoteVersionLinksByVersionId_delete
      x-api-path-slug: api2versionversionidremotelink-delete
      parameters:
      - in: path
        name: versionId
        description: The version for which to delete ALL existing remote version links
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Links
      - By
      - Version
      - Id
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