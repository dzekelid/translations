{
  "info": {
    "name": "Giphy Gif API Translate phrase to Sticker",
    "_postman_id": "852519e7-05ee-479b-9a21-6bae71bdf858",
    "description": "The translate API draws on search, but uses the GIPHY `special sauce` to handle translating from one vocabulary to another. In this case, words and phrases to GIFs.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "stickers",
      "item": [
        {
          "id": "a750fcb6-9254-4f22-849f-df083ae6cb6e",
          "name": "translateSticker",
          "request": {
            "url": "http://api.giphy.com/v1/stickers/translate?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The translate API draws on search, but uses the GIPHY `special sauce` to handle translating from one vocabulary to another"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "701d5b9c-9423-41a7-ab42-7163e67f4d3f"
            }
          ]
        }
      ]
    }
  ]
}