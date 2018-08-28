swagger: "2.0"
x-collection-name: Giphy
x-complete: 1
info:
  title: Giphy
  description: natively-embed-all-the-best-features-of-the-worlds-largest-and-most-powerful-gif-library-into-your-app-
  termsOfService: https://developers.giphy.com/
  version: v1
host: api.giphy.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gifs/translate:
    get:
      summary: Translate phrase to GIF
      description: The translate API draws on search, but uses the GIPHY `special
        sauce` to handle translating from one vocabulary to another. In this case,
        words and phrases to GIF
      operationId: translateGif
      x-api-path-slug: gifstranslate-get
      parameters:
      - in: query
        name: No Name
      responses:
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Gifs
      - Translate
  /stickers/translate:
    get:
      summary: Translate phrase to Sticker
      description: The translate API draws on search, but uses the GIPHY `special
        sauce` to handle translating from one vocabulary to another. In this case,
        words and phrases to GIFs.
      operationId: translateSticker
      x-api-path-slug: stickerstranslate-get
      parameters:
      - in: query
        name: No Name
      responses:
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Stickers
      - Translate