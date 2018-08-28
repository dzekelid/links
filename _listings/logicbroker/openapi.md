swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Orders/{LogicbrokerKey}/Invoices:
    post:
      summary: Creates invoice and links with the given order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_CreateInvoiceForSalesOrder
      x-api-path-slug: apiv1orderslogicbrokerkeyinvoices-post
      parameters:
      - in: body
        name: Invoice
        description: The invoice
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Invoice
      - Links
      - Given
      - Order