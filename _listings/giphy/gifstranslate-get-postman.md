{
  "info": {
    "name": "Giphy Gif API Translate phrase to GIF",
    "_postman_id": "cb66321f-a97a-43ef-94c7-999a70725b16",
    "description": "The translate API draws on search, but uses the GIPHY `special sauce` to handle translating from one vocabulary to another. In this case, words and phrases to GIF",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gifs",
      "item": [
        {
          "id": "1840e327-fb77-4d19-bc8f-bb6755c34168",
          "name": "getGifsById",
          "request": {
            "url": "http://api.giphy.com/v1/gifs?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A multiget version of the get GIF by ID endpoint."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "65000b0b-5b46-4266-9270-381eb10e25ac"
            }
          ]
        },
        {
          "id": "8f0b1fc0-c34e-45ba-a8db-3baf554dbe3d",
          "name": "randomGif",
          "request": {
            "url": "http://api.giphy.com/v1/gifs/random?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a random GIF, limited by tag. Excluding the tag parameter will return a random GIF from the GIPHY catalog."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "a900b02b-ff95-4de5-a169-00fbe5506d22"
            }
          ]
        },
        {
          "id": "a0f1e00f-a146-4f17-89d1-b8ebd0e7a1d1",
          "name": "searchGifs",
          "request": {
            "url": "http://api.giphy.com/v1/gifs/search?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search all GIPHY GIFs for a word or phrase. Punctuation will be stripped and ignored.  Use a plus or url encode for phrases. Example paul+rudd, ryan+gosling or american+psycho."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "099c8593-72dd-44f3-8f14-09548b3a16b8"
            }
          ]
        },
        {
          "id": "2c79477d-560e-4a46-add2-200e60c036ef",
          "name": "translateGif",
          "request": {
            "url": "http://api.giphy.com/v1/gifs/translate?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The translate API draws on search, but uses the GIPHY `special sauce` to handle translating from one vocabulary to another. In this case, words and phrases to GIF"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "2f31291f-381e-447e-abf4-21407bde7bcb"
            }
          ]
        }
      ]
    }
  ]
}