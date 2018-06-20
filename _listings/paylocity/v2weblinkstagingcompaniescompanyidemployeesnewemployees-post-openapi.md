---
swagger: "2.0"
x-collection-name: Paylocity
x-complete: 0
info:
  title: Paylocity Add new employee to Web Link
  description: Add new employee to Web Link will send partially completed or potentially
    erroneous new hire record to Web Link, where it can be corrected and competed
    by company administrator or authorized Paylocity Service Bureau employee.
  termsOfService: WebLink.OpenApiDoc.TermsOfService
  version: "2"
host: api.paylocity.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/weblinkstaging/companies/{companyId}/employees/newemployees:
    post:
      summary: Add new employee to Web Link
      description: Add new employee to Web Link will send partially completed or potentially
        erroneous new hire record to Web Link, where it can be corrected and competed
        by company administrator or authorized Paylocity Service Bureau employee.
      operationId: v2.weblinkstaging.companies.companyId.employees.newemployees.post
      x-api-path-slug: v2weblinkstagingcompaniescompanyidemployeesnewemployees-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: body
        name: json
        description: StagedEmployee Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Weblinkstaging
      - Companies
      - CompanyId
      - Employees
      - Newemployees
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