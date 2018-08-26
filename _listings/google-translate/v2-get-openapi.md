---
swagger: "2.0"
x-collection-name: Google Translate
x-complete: 0
info:
  title: Google Translate API Translate Text
  description: Returns text translations from one language to another.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /language/translate
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2:
    get:
      summary: Translate Text
      description: Returns text translations from one language to another.
      operationId: language.translations.list
      x-api-path-slug: v2-get
      parameters:
      - in: query
        name: cid
        description: The customization id for translate
      - in: query
        name: format
        description: The format of the text
      - in: query
        name: q
        description: The text to translate
      - in: query
        name: source
        description: The source language of the text
      - in: query
        name: target
        description: The target language into which the text should be translated
      responses:
        200:
          description: OK
      tags:
      - Translate
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