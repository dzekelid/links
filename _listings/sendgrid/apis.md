---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "10000"
tags: Links
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid Get Whitelabel Links
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all link whitelabels.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links
  tags: Email,Whitelabel, Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinks-get-openapi.md
- name: SendGrid Add Whitelabel Links
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a new link whitelabel.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links
  tags: Email,Whitelabel, Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinks-post-openapi.md
- name: SendGrid Get Whitelabel Links Default
  x-api-slug: sendgrid
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/default
  tags: Email,Whitelabel, Links, Default
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinksdefault-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinksdefault-get-openapi.md
- name: SendGrid Delete Whitelabel Links Subuser
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to disassociate a link whitelabel from a subuser.**

    Link whitelables can be associated with subusers from the parent account. This functionality allows
    subusers to send mail using their parent's linke whitelabels. To associate a link whitelabel, the parent account
    must first create a whitelabel and validate it. The parent may then associate that whitelabel with a subuser via the API or the Subuser Management page in the user interface.

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/subuser
  tags: Email,Whitelabel, Links, Subuser
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinkssubuser-delete-openapi.md
- name: SendGrid Get Whitelabel Links Subuser
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the associated link whitelabel for a subuser.**

    Link whitelables can be associated with subusers from the parent account. This functionality allows
    subusers to send mail using their parent's linke whitelabels. To associate a link whitelabel, the parent account
    must first create a whitelabel and validate it. The parent may then associate that whitelabel with a subuser via the API or the Subuser Management page in the user interface.

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/subuser
  tags: Email,Whitelabel, Links, Subuser
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinkssubuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinkssubuser-get-openapi.md
- name: SendGrid Delete Whitelabel Links
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a link whitelabel.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/{id}
  tags: Email,Whitelabel, Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinksid-delete-openapi.md
- name: SendGrid Get Whitelabel Links
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a specific link whitelabel.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/{id}
  tags: Email,Whitelabel, Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinksid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinksid-get-openapi.md
- name: SendGrid Patch Whitelabel Links
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update a specific link whitelabel. You can use this endpoint to change a link whitelabel's default status.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/{id}
  tags: Email,Whitelabel, Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinksid-patch-openapi.md
- name: SendGrid Add Whitelabel Links  Valate
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to validate a link whitelabel.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/{id}/validate
  tags: Email,Whitelabel, Links, , Valate
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinksidvalidate-post-openapi.md
- name: SendGrid Add Whitelabel Links Link  Subuser
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to associate a link whitelabel with a subuser account.**

    Link whitelables can be associated with subusers from the parent account. This functionality allows
    subusers to send mail using their parent's linke whitelabels. To associate a link whitelabel, the parent account
    must first create a whitelabel and validate it. The parent may then associate that whitelabel with a subuser via the API or the Subuser Management page in the user interface.

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/{link_id}/subuser
  tags: Email,Whitelabel, Links, Link, , Subuser
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/whitelabellinkslink-idsubuser-post-openapi.md
- name: SendGrid
  x-api-slug: sendgrid
  description: SendGrids cloud-based email infrastructure relieves businesses of the
    cost and complexity of maintaining custom email systems. SendGrid provides reliable
    delivery, scalability and real-time analytics along with flexible APIs that make
    custom integration a breeze.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/sendgrid/openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-linkedin
  url: https://www.linkedin.com/company/sendgrid
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---