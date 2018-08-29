---
swagger: "2.0"
x-collection-name: TransitFeeds
x-complete: 0
info:
  title: TransitFeeds Retrieve a list of versions of specified (or all) feeds.
  description: |-
    This API call allows you to easily see every single feed update in the TranstiFeeds.com system. Since this can be quite
    long, it's also possible to filter this list by a single feed ID.
  contact:
    name: TransitFeeds.com
    url: https://transitfeeds.com/issues
    email: support@transitfeeds.com
  version: 1.0.0
host: api.transitfeeds.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /getFeedVersions:
    get:
      summary: Retrieve a list of versions of specified (or all) feeds.
      description: |-
        This API call allows you to easily see every single feed update in the TranstiFeeds.com system. Since this can be quite
        long, it's also possible to filter this list by a single feed ID.
      operationId: getFeedVersions
      x-api-path-slug: getfeedversions-get
      parameters:
      - in: query
        name: err
        description: To include any errors detected when importing this feed in the
          response, specify a valud of `1`
      - in: query
        name: feed
        description: If you only want to retrieve feed versions for a particular feed,
          include its ID here
      - in: query
        name: key
        description: Your personal API key, used for authentication
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: page
        description: The page number of results to return
      - in: query
        name: warn
        description: To include any warnings detected when importing this feed in
          the response, specify a valud of `1`
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Versions
      - Of
      - Specified
      - (or
      - )
      - Feeds
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