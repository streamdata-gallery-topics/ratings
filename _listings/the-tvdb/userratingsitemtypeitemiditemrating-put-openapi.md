---
swagger: "2.0"
x-collection-name: The TVDB
x-complete: 0
info:
  title: The TVDB Put User Ratings Itemtype Itemid Itemrating
  description: This route updates a given rating of a given type.
  version: 2.1.2
host: api-dev.thetvdb.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/ratings:
    get:
      summary: Get User Ratings
      description: Returns an array of ratings for the given user.
      operationId: user.ratings.get
      x-api-path-slug: userratings-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
  /user/ratings/query:
    get:
      summary: Get User Ratings Query
      description: Returns an array of ratings for a given user that match the query.
      operationId: user.ratings.query.get
      x-api-path-slug: userratingsquery-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
      - Query
  /user/ratings/query/params:
    get:
      summary: Get User Ratings Query Params
      description: Returns a list of query params for use in the `/user/ratings/query`
        route.
      operationId: user.ratings.query.params.get
      x-api-path-slug: userratingsqueryparams-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
      - Query
      - Params
  /user/ratings/{itemType}/{itemId}:
    delete:
      summary: Delete User Ratings Itemtype Itemid
      description: This route deletes a given rating of a given type.
      operationId: user.ratings.itemType.itemId.delete
      x-api-path-slug: userratingsitemtypeitemid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
      - ItemType
      - ItemId
  /user/ratings/{itemType}/{itemId}/{itemRating}:
    put:
      summary: Put User Ratings Itemtype Itemid Itemrating
      description: This route updates a given rating of a given type.
      operationId: user.ratings.itemType.itemId.itemRating.put
      x-api-path-slug: userratingsitemtypeitemiditemrating-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
      - ItemType
      - ItemId
      - ItemRating
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