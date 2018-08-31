---
swagger: "2.0"
x-collection-name: Framesocket
x-complete: 0
info:
  title: Framesocket Deactive Media
  description: Deactive Media
  version: 1.0.0
host: www.framesocket.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/activate.php:
    get:
      summary: Activate Media
      description: Activate Media
      operationId: getMediaActivate.php
      x-api-path-slug: mediaactivate-php-get
      parameters:
      - in: query
        name: customid
        description: Custom ID
      - in: query
        name: hash
        description: Video Hash
      - in: query
        name: key
        description: Your account username
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      responses:
        200:
          description: OK
      tags:
      - Media
      - Activate
  /media/deactivate.php:
    get:
      summary: Deactive Media
      description: Deactive Media
      operationId: getMediaDeactivate.php
      x-api-path-slug: mediadeactivate-php-get
      parameters:
      - in: query
        name: customid
        description: Custom ID
      - in: query
        name: hash
        description: Video Hash
      - in: query
        name: key
        description: Your account username
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      responses:
        200:
          description: OK
      tags:
      - Media
      - Deactivate
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