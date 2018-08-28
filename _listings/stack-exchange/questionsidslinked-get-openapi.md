---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get Question Linked
  description: "Gets questions which link to those questions identified in {ids}.\n
    \nThis method only considers questions that are linked within a site, and will
    never return questions from another Stack Exchange site.\n \nA question is considered
    \"linked\" when it explicitly includes a hyperlink to another question, there
    are no other heuristics.\n \n{ids} can contain up to 100 semicolon delimited ids,
    to find ids programatically look for question_id on question objects.\n \nThe
    sorts accepted by this method operate on the follow fields of the question object:\n
    - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
    - rank - a priority sort by site applies, subject to change at any time Does not
    accept min or max\n  activity is the default sort.\n \n It is possible to create
    moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
    method returns a list of questions."
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
  /questions/{ids}/comments:
    get:
      summary: Get Question Comments
      description: "Gets the comments on a question.\n \nIf you know that you have
        an question id and need the comments, use this method. If you know you have
        a answer id, use /answers/{ids}/comments. If you are unsure, use /posts/{ids}/comments.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for question_id on question objects.\n \nThe sorts accepted by this method
        operate on the follow fields of the comment object:\n - creation - creation_date\n
        - votes - score\n  creation is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of comments."
      operationId: gets-the-comments-on-a-question-if-you-know-that-you-have-an-question-id-and-need-the-comments-use-t
      x-api-path-slug: questionsidscomments-get
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
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
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
      - Linked
  /questions/{ids}/linked:
    get:
      summary: Get Question Linked
      description: "Gets questions which link to those questions identified in {ids}.\n
        \nThis method only considers questions that are linked within a site, and
        will never return questions from another Stack Exchange site.\n \nA question
        is considered \"linked\" when it explicitly includes a hyperlink to another
        question, there are no other heuristics.\n \n{ids} can contain up to 100 semicolon
        delimited ids, to find ids programatically look for question_id on question
        objects.\n \nThe sorts accepted by this method operate on the follow fields
        of the question object:\n - activity - last_activity_date\n - creation - creation_date\n
        - votes - score\n - rank - a priority sort by site applies, subject to change
        at any time Does not accept min or max\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of questions."
      operationId: gets-questions-which-link-to-those-questions-identified-in-ids-this-method-only-considers-questions-
      x-api-path-slug: questionsidslinked-get
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
      - Linked
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