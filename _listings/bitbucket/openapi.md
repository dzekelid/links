swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 1
info:
  title: Bitbucket
  description: code-against-the-bitbucket-api-to-automate-simple-tasks-embed-bitbucket-data-into-your-own-site-build-mobile-or-desktop-apps-or-even-add-custom-ui-addons-into-bitbucket-itself-using-the-connect-framework-
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /addon/linkers:
    get:
      summary: Get Add On Linkers
      description: Get addon linkers
      operationId: getAddonLinkers
      x-api-path-slug: addonlinkers-get
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
    parameters:
      summary: Parameters Add On Linkers
      description: Parameters addon linkers
      operationId: parametersAddonLinkers
      x-api-path-slug: addonlinkers-parameters
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
  /addon/linkers/{linker_key}:
    get:
      summary: Get Add On Linkers Linker Key
      description: Get addon linkers linker key
      operationId: getAddonLinkersLinkerKey
      x-api-path-slug: addonlinkerslinker-key-get
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
      - Linker
      - Key
    parameters:
      summary: Parameters Add On Linkers Linker Key
      description: Parameters addon linkers linker key
      operationId: parametersAddonLinkersLinkerKey
      x-api-path-slug: addonlinkerslinker-key-parameters
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
      - Linker
      - Key
  /addon/linkers/{linker_key}/values:
    delete:
      summary: Delete Add On Linkers Linker Key Values
      description: Delete addon linkers linker key values
      operationId: deleteAddonLinkersLinkerKeyValues
      x-api-path-slug: addonlinkerslinker-keyvalues-delete
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
      - Linker
      - Key
      - Values
    get:
      summary: Get Add On Linkers Linker Key Values
      description: Get addon linkers linker key values
      operationId: getAddonLinkersLinkerKeyValues
      x-api-path-slug: addonlinkerslinker-keyvalues-get
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
      - Linker
      - Key
      - Values
    parameters:
      summary: Parameters Add On Linkers Linker Key Values
      description: Parameters addon linkers linker key values
      operationId: parametersAddonLinkersLinkerKeyValues
      x-api-path-slug: addonlinkerslinker-keyvalues-parameters
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
      - Linker
      - Key
      - Values
    post:
      summary: Add Add On Linkers Linker Key Values
      description: Post addon linkers linker key values
      operationId: postAddonLinkersLinkerKeyValues
      x-api-path-slug: addonlinkerslinker-keyvalues-post
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
      - Linker
      - Key
      - Values
    put:
      summary: Update Add On Linkers Linker Key Values
      description: Put addon linkers linker key values
      operationId: putAddonLinkersLinkerKeyValues
      x-api-path-slug: addonlinkerslinker-keyvalues-put
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
      - Linker
      - Key
      - Values
  /addon/linkers/{linker_key}/values/:
    delete:
      summary: Delete Add On Linkers Linker Key Values
      description: Delete addon linkers linker key values
      operationId: deleteAddonLinkersLinkerKeyValues
      x-api-path-slug: addonlinkerslinker-keyvalues-delete
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
      - Linker
      - Key
      - Values
    get:
      summary: Get Add On Linkers Linker Key Values
      description: Get addon linkers linker key values
      operationId: getAddonLinkersLinkerKeyValues
      x-api-path-slug: addonlinkerslinker-keyvalues-get
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
      - Linker
      - Key
      - Values
    parameters:
      summary: Parameters Add On Linkers Linker Key Values
      description: Parameters addon linkers linker key values
      operationId: parametersAddonLinkersLinkerKeyValues
      x-api-path-slug: addonlinkerslinker-keyvalues-parameters
      responses:
        200:
          description: OK
      tags:
      - Addon
      - Linkers
      - Linker
      - Key
      - Values