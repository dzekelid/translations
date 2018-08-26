---
swagger: "2.0"
x-collection-name: SAP
x-complete: 1
info:
  title: SAP Translation Hub
  description: to-provide-users-of-software-in-a-global-market-with-texts-in-their-own-language-translations-are-required--sap-translation-hub-enables-you-to-draw-on-saps-translation-experience-across-multiple-products-and-languages-to-propose-translations-for-short-texts-
  contact:
    name: SAP Translation Hub team
    email: translationhub@sap.com
  version: 1.0.0
host: sandbox.api.sap.com
basePath: /translationhub/api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /translate:
    post:
      summary: The '/translate' resource enables you to get translations of English
        short texts that exist in SAP Translation Hub.
      description: Provides translations of short texts based on a combination of
        existing texts and their translations that are used in SAP products and machine
        translation capabilities.
      operationId: provides-translations-of-short-texts-based-on-a-combination-of-existing-texts-and-their-translations
      x-api-path-slug: translate-post
      parameters:
      - in: header
        name: Content-Type
        description: Specifies the nature of the data in the body so that the receiving
          agent can process the data accordingly
      - in: body
        name: translate
        description: The JSON request contains an array of ```units``` JSON objects
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - The
      - ""
      - Translate
      - Resource
      - Enables
      - You
      - To
      - Get
      - Translations
      - Of
      - English
      - Short
      - Texts
      - That
      - Exist
      - In
      - SAP
      - Translation
      - Hub
  /languages:
    get:
      summary: Languages that SAP Translation Hub supports.
      description: Returns a list of the languages that SAP Translation Hub supports.
        You can also check whether a particualr language is available in SAP Translation
        Hub.
      operationId: returns-a-list-of-the-languages-that-sap-translation-hub-supports-you-can-also-check-whether-a-parti
      x-api-path-slug: languages-get
      parameters:
      - in: header
        name: Content-Type
        description: Specifies the nature of the data in the body so that the receiving
          agent can process the data accordingly
      - in: query
        name: search
        description: Determines whether a particular language is available in SAP
          Translation Hub
      responses:
        200:
          description: Successful response
      tags:
      - Languages
      - That
      - SAP
      - Translation
      - Hub
      - Supports
  /texttypes:
    get:
      summary: Returns a list of the text types available in SAP Translation Hub.
      description: In SAP products, short texts, such as those used on user interfaces
        (UIs), are characterized by various text types. The type of a specific text
        is determined by the UI element that it describes. For example,  button texts
        are described by the text type ```XBUT```. <br> The text type resource returns
        a list of the text types that are available in SAP Translation Hub. You can
        combine the '/text type' resource with the '/suggestion' resource to narrow
        down the results of the suggestion resource.
      operationId: in-sap-products-short-texts-such-as-those-used-on-user-interfaces-uis-are-characterized-by-various-t
      x-api-path-slug: texttypes-get
      parameters:
      - in: header
        name: Content-Type
        description: Specifies the nature of the data in the body so that the receiving
          agent can process the data accordingly
      - in: query
        name: search
        description: Allows you to search for a specific text type, such as message
      responses:
        200:
          description: Successful response
      tags:
      - Returns
      - List
      - Of
      - Text
      - Types
      - Available
      - In
      - SAP
      - Translation
      - Hub
---