---
name: Paylocity
x-slug: paylocity
description: ""
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Links
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/paylocity/apis.md
specificationVersion: "0.14"
apis:
- name: Paylocity Add new employee to Web Link
  x-api-slug: paylocity
  description: Add new employee to Web Link will send partially completed or potentially
    erroneous new hire record to Web Link, where it can be corrected and competed
    by company administrator or authorized Paylocity Service Bureau employee.
  image: ""
  humanURL: http://paylocity.com
  baseURL: https://api.paylocity.com//api//v2/weblinkstaging/companies/{companyId}/employees/newemployees
  tags: V2,Weblinkstaging,Companies,CompanyId,Employees,Newemployees
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/paylocity/v2weblinkstagingcompaniescompanyidemployeesnewemployees-post-openapi.md
- name: Paylocity
  x-api-slug: paylocity
  description: ""
  image: ""
  humanURL: http://paylocity.com
  baseURL: https://api.paylocity.com//api
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/paylocity/openapi.md
x-common:
- type: x-blog
  url: https://www.paylocity.com/resources/blog/
- type: x-github
  url: https://github.com/Paylocity
- type: x-integrations
  url: https://www.paylocity.com/partnerships/integrations/
- type: x-twitter
  url: https://twitter.com/Paylocity
- type: x-website
  url: http://paylocity.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---