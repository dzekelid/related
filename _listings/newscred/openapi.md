---
swagger: "2.0"
x-collection-name: NewsCred
x-complete: 1
info:
  title: News Cred
  description: returns-a-list-of-articles-according-to-the-specified-set-of-parameters-
  version: v1
host: api.newscred.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  topics/related/:
    get:
      summary: Related Topics
      description: Given some search criteria, returns a list of topics related to
        those criteria.
      operationId: getTopicsRelated
      x-api-path-slug: topicsrelated-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: from_date, to_date
        description: Find topics that were trending (written about more than usual)
          during the specified date range
      - in: query
        name: offset
        description: Number of topics to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of topics to return
      - in: query
        name: query
        description: Find topics related to these keywords
      - in: query
        name: topics
        description: List of topics to retrieve items from
      - in: query
        name: topic_classifications
        description: Limit results to those with the specified topic classification
      - in: query
        name: topic_filter_mode
        description: Enables topic_filter_name and indicates filtering type
      - in: query
        name: topic_filter_name
        description: Limit items to a predefined list of topics
      - in: query
        name: topic_subclassifications
        description: Limit results to those with the specified topic sub-classification
      responses:
        200:
          description: OK
      tags:
      - News
      - Topics
      - Related
---