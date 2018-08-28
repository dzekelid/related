---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get Question Related
  description: "Returns questions that the site considers related to those identified
    in {ids}.\n \nThe algorithm for determining if questions are related is not documented,
    and subject to change at any time. Futhermore, these values are very heavily cached,
    and may not update immediately after a question has been editted. It is also not
    guaranteed that a question will be considered related to any number (even non-zero)
    of questions, and a consumer should be able to handle a variable number of returned
    questions.\n \n{ids} can contain up to 100 semicolon delimited ids, to find ids
    programatically look for question_id on question objects.\n \nThe sorts accepted
    by this method operate on the follow fields of the question object:\n - activity
    - last_activity_date\n - creation - creation_date\n - votes - score\n - rank -
    a priority sort by site applies, subject to change at any time Does not accept
    min or max\n  activity is the default sort.\n \n It is possible to create moderately
    complex queries using sort, min, max, fromdate, and todate.\n \nThis method returns
    a list of questions."
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /questions/{ids}/related:
    get:
      summary: Get Question Related
      description: "Returns questions that the site considers related to those identified
        in {ids}.\n \nThe algorithm for determining if questions are related is not
        documented, and subject to change at any time. Futhermore, these values are
        very heavily cached, and may not update immediately after a question has been
        editted. It is also not guaranteed that a question will be considered related
        to any number (even non-zero) of questions, and a consumer should be able
        to handle a variable number of returned questions.\n \n{ids} can contain up
        to 100 semicolon delimited ids, to find ids programatically look for question_id
        on question objects.\n \nThe sorts accepted by this method operate on the
        follow fields of the question object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n - rank - a priority sort by
        site applies, subject to change at any time Does not accept min or max\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: returns-questions-that-the-site-considers-related-to-those-identified-in-ids-the-algorithm-for-deter
      x-api-path-slug: questionsidsrelated-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = rank => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = rank => none
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
      - Related
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