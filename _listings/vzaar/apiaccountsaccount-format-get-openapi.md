---
swagger: "2.0"
x-collection-name: Vzaar
x-complete: 0
info:
  title: Vzaar API Get Api Accounts Account
  description: 'nnThis API call returns the details and rights for each vzaar subscription
    account type along with its relevant metadata. This will show the details of the
    packages available here: http://vzaar.com/pricingnn'
  termsOfService: http://vzaar.com/policies
  version: v1
host: vzaar.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounts/{account}.{format}:
    get:
      summary: Get Api Accounts Account
      description: 'nnThis API call returns the details and rights for each vzaar
        subscription account type along with its relevant metadata. This will show
        the details of the packages available here: http://vzaar.com/pricingnn'
      operationId: getApiAccountsAccount.Format
      x-api-path-slug: apiaccountsaccount-format-get
      parameters:
      - in: query
        name: account is the vzaar account type. This is an integer.
      responses:
        200:
          description: OK
      tags:
      - Api
      - Accounts
      - Account
      - Format
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