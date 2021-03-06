---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Remove additional service to lettings role tenancy
  version: 1.0.0
  description: Remove additional service to lettings role tenancy.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounting/exports/batch/{id}/removepayment:
    put:
      summary: Remove an individual payment from batch export
      description: Remove an individual payment from batch export.
      operationId: AccountingExport_RemoveFromBatchByidBypaymentId
      x-api-path-slug: apiaccountingexportsbatchidremovepayment-put
      parameters:
      - in: path
        name: id
      - in: query
        name: paymentId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Individual
      - Payment
      - From
      - Batch
      - Export
  /api/auction/removecontact:
    post:
      summary: Remove an existing auction contact from the auction role
      description: Remove an existing auction contact from the auction role.
      operationId: Auction_RemoveAuctionContactByremoveContactDataContract
      x-api-path-slug: apiauctionremovecontact-post
      parameters:
      - in: body
        name: removeContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Existing
      - Auction
      - Contact
      - From
      - Auction
      - Role
  /api/dashboard/{id}/removewidgets:
    put:
      summary: Remove widgets from a dashboard
      description: Remove widgets from a dashboard.
      operationId: Dashboard_RemoveWidgetsFromDashboardByid
      x-api-path-slug: apidashboardidremovewidgets-put
      parameters:
      - in: path
        name: id
        description: Dashboard Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Widgets
      - From
      - Dashboard
  /api/group/{id}/removepreferredcompany:
    post:
      summary: Remove a preferred company to a group
      description: Remove a preferred company to a group.
      operationId: Group_RemovePreferredCompanyByidBycompanyId
      x-api-path-slug: apigroupidremovepreferredcompany-post
      parameters:
      - in: query
        name: companyId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Preferred
      - Company
      - To
      - Group
  /api/invoice/{id}/removefee:
    put:
      summary: Remove fee from existing invoice
      description: Remove fee from existing invoice.
      operationId: Invoice_RemoveLinkedFeeByidByattachedFeeId
      x-api-path-slug: apiinvoiceidremovefee-put
      parameters:
      - in: query
        name: attachedFeeId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Fee
      - From
      - Existing
      - Invoice
  /api/invoice/removereceiptallocation:
    delete:
      summary: Remove a receipt list item allocation
      description: Remove a receipt list item allocation.
      operationId: Invoice_RemoveSavedReceiptItemAllocationByreceiptItemIdByinvoiceIdByallocationId
      x-api-path-slug: apiinvoiceremovereceiptallocation-delete
      parameters:
      - in: query
        name: allocationId
      - in: query
        name: invoiceId
      - in: query
        name: receiptItemId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Receipt
      - List
      - Item
      - Ocation
  /api/role/lettings/{roleId}/removeutility:
    delete:
      summary: Remove a utility for the letting role
      description: Remove a utility for the letting role.
      operationId: LettingRole_RemoveUtilityUtilityByroleIdByutilityId
      x-api-path-slug: apirolelettingsroleidremoveutility-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: The letting role Id
      - in: query
        name: utilityId
        description: The utility Id
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Utilitythe
      - Letting
      - Role
  /api/role/lettings/{id}/removeadditionalservice/{additionalServiceId}:
    post:
      summary: Remove additional service to lettings role tenancy
      description: Remove additional service to lettings role tenancy.
      operationId: LettingRole_DeleteAdditionalServiceByidByadditionalServiceId
      x-api-path-slug: apirolelettingsidremoveadditionalserviceadditionalserviceid-post
      parameters:
      - in: path
        name: additionalServiceId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Additional
      - Service
      - To
      - Lettings
      - Role
      - Tenancy
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