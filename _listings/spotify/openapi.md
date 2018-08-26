---
swagger: "2.0"
x-collection-name: Spotify
x-complete: 1
info:
  title: Spotify
  description: our-web-api-lets-your-applications-fetch-data-from-the-spotify-music-catalog-and-manage-users-playlists-and-saved-music--based-on-simple-rest-principles-our-web-api-endpoints-return-metadata-in-json-format-about-artists-albums-and-tracks-directly-from-the-spotify-catalogue--the-api-also-provides-access-to-userrelated-data-such-as-playlists-and-music-saved-in-a-your-music-library-subject-to-users-authorization-
  version: v1
host: api.spotify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /artists/{id}/related-artists:
    get:
      summary: Get Artist Related ARtists
      description: '[Get an Artist''s Related Artists](https://developer.spotify.com/web-api/get-related-artists/)'
      operationId: get-an-artists-related-artistshttpsdeveloperspotifycomwebapigetrelatedartists
      x-api-path-slug: artistsidrelatedartists-get
      parameters:
      - in: path
        name: id
        description: The Spotify ID for the artist
      responses:
        200:
          description: OK
      tags:
      - Music
      - Artists
---