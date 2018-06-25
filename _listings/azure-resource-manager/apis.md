---
name: Azure Resource Manager
x-slug: azure-resource-manager
description: Azure Resource Manager enables you to deploy and manage the infrastructure
  for your Azure solutions. You organize related resources in resource groups, and
  deploy your resources with JSON templates. For an introduction to deploying and
  managing resources with Resource Manager, see Azure Resource Manager overview.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Links
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Resource Manager API Resource Links Delete
  x-api-slug: azure-resource-manager-api
  description: Deletes a resource link with the specified ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{linkId}
  tags: Resource Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/linkid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/linkid-delete-openapi.md
- name: Azure Resource Manager API Resource Links Create Or Update
  x-api-slug: azure-resource-manager-api
  description: Creates or updates a resource link between the specified resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{linkId}
  tags: Resource Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/linkid-put-openapi.md
- name: Azure Resource Manager API Resource Links Get
  x-api-slug: azure-resource-manager-api
  description: Gets a resource link with the specified ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{linkId}
  tags: Resource Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/linkid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/linkid-get-openapi.md
- name: Azure Resource Manager API Resource Links List At Subscription
  x-api-slug: azure-resource-manager-api
  description: Gets all the linked resources for the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Resources/links
  tags: Resource Links At Subscription
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get-openapi.md
- name: Azure Resource Manager API Resource Links List At Source Scope
  x-api-slug: azure-resource-manager-api
  description: Gets a list of resource links at and below the specified source scope.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Resources/links
  tags: Resource Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-resourceslinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-resourceslinks-get-openapi.md
- name: Azure Resource Manager API
  x-api-slug: azure-resource-manager-api
  description: Azure Resource Manager enables you to deploy and manage the infrastructure
    for your Azure solutions. You organize related resources in resource groups, and
    deploy your resources with JSON templates. For an introduction to deploying and
    managing resources with Resource Manager, see Azure Resource Manager overview.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/azure-resource-manager/openapi.md
x-common:
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---