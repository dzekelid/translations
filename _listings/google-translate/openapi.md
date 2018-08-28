swagger: "2.0"
x-collection-name: Google Translate
x-complete: 1
info:
  title: Translate
  description: translates-text-from-one-language-to-another-
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