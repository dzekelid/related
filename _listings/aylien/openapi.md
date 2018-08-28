swagger: "2.0"
x-collection-name: Aylien
x-complete: 1
info:
  title: AYLIEN News API
  description: the-aylien-news-api-is-the-most-powerful-way-of-sourcing-searching-and-syndicating-analyzed-and-enriched-news-content--it-is-accessed-by-sending-http-requests-to-our-server-which-returns-information-to-your-client-
  termsOfService: https://newsapi.aylien.com/tos
  contact:
    name: API support
    url: https://newsapi.aylien.com/
    email: support@aylien.com
  version: 1.0.0
host: api.newsapi.aylien.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /related_stories:
    get:
      summary: List related stories
      description: This endpoint is used for finding semantically similar stories
        based on the parameters you provide as inputs. For example, if you want to
        find stories similar to a Tweet or any text extract you input, the related
        stories endpoint will analyze the entities present and the meaning of the
        text, and find stories with a similar meaning. The maximum number of related
        stories returned is 100.
      operationId: listRelatedStories
      x-api-path-slug: related-stories-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - News
      - List
      - Related
      - Stories
    post:
      summary: List related stories
      description: This endpoint is used for finding semantically similar stories
        based on the parameters you provide as inputs. For example, if you want to
        find stories similar to a Tweet or any text extract you input, the related
        stories endpoint will analyze the entities present and the meaning of the
        text, and find stories with a similar meaning. The maximum number of related
        stories returned is 100.
      operationId: listRelatedStoriesAsPost
      x-api-path-slug: related-stories-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - News
      - List
      - Related
      - Stories