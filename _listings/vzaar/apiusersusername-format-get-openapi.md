---
swagger: "2.0"
x-collection-name: Vzaar
x-complete: 0
info:
  title: Vzaar API Get Api Users Username
  description: nnThis API call returns the users public details along with its relevant
    metadata.nn
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
  /api/upload/link.xmln:
    post:
      summary: Post Api Upload Link.xmln
      description: nnThis API call allows a user to upload &amp; process video file
        from given url.nn
      operationId: postApiUploadLink.xmln
      x-api-path-slug: apiuploadlink-xmln-post
      parameters:
      - in: query
        name: bitrate
        description: Specifies videos bitrate
      - in: query
        name: description
        description: Specifies the description for the video
      - in: query
        name: encoding_params
        description: Includes optional parameters
      - in: query
        name: guid
        description: Specifies the guid to operate on
      - in: query
        name: key
        description: A name for the S3 object that stores the uploaded file
      - in: query
        name: size_id
        description: Specifies the size for the video to be encoded in
      - in: query
        name: title
        description: Specifies the title for the video
      - in: query
        name: transcoding
        description: True forces vzaar to transcode the video, false makes vzaar use
          the original source file
      - in: query
        name: url
        description: Specifies the url to video file
      - in: query
        name: width
        description: Specifies videos width
      - in: query
        name: XML/JSON
      responses:
        200:
          description: OK
      tags:
      - Api
      - Upload
      - Link
      - Xmln
  /api/users/{username}.{format}:
    get:
      summary: Get Api Users Username
      description: nnThis API call returns the users public details along with its
        relevant metadata.nn
      operationId: getApiUsersUsername.Format
      x-api-path-slug: apiusersusername-format-get
      parameters:
      - in: query
        name: 'username is the vzaar login name for the user. Note: This must be the
          actual username and not the email address'
      responses:
        200:
          description: OK
      tags:
      - Api
      - Users
      - Username
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