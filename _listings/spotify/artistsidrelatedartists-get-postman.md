{
  "info": {
    "name": "Spotify",
    "_postman_id": "41031df9-4224-4439-adda-393c468a87a3",
    "description": "Our Web API lets your applications fetch data from the Spotify music catalog and manage user&rsquo;s playlists and saved music. Based on simple REST principles, our Web API endpoints return metadata in JSON format about artists, albums, and tracks directly from the Spotify catalogue. The API also provides access to user-related data such as playlists and music saved in a &ldquo;Your Music&rdquo; library, subject to user&rsquo;s authorization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "b225e24c-92e2-4905-82c1-11ab5ec483a3",
          "name": "get-an-artists-related-artistshttpsdeveloperspotifycomwebapigetrelatedartists",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spotify.com",
              "path": [
                "v1",
                "artists/:id/related-artists"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "[Get an Artist's Related Artists](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06efe1ac-3590-4e37-8dcc-41077c734f0e"
            }
          ]
        }
      ]
    }
  ]
}