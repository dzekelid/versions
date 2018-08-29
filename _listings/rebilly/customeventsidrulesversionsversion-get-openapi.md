---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Retrieve the version of the set of rules for a custom event
  description: |-
    Retrieve the version of the selected set of rules for the selected custom event.
    The versions are created each time you change the rules.
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /custom-events/{id}/rules/versions/{version}:
    get:
      summary: Retrieve the version of the set of rules for a custom event
      description: |-
        Retrieve the version of the selected set of rules for the selected custom event.
        The versions are created each time you change the rules.
      operationId: retrieve-the-version-of-the-selected-set-of-rules-for-the-selected-custom-event-the-versions-are-cre
      x-api-path-slug: customeventsidrulesversionsversion-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Version
      - Of
      - Set
      - Of
      - Rulesa
      - Custom
      - Event
  /events/{eventType}/rules/versions/{version}:
    get:
      summary: Retrieve the version of the set of rules
      description: |-
        Retrieve the version of the selected set of rules.
        The versions are created each time you change the rules.
      operationId: retrieve-the-version-of-the-selected-set-of-rules-the-versions-are-created-each-time-you-change-the-
      x-api-path-slug: eventseventtyperulesversionsversion-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Version
      - Of
      - Set
      - Of
      - Rules
  /lists:
    get:
      summary: Retrieve a collection of Lists (latest version of each List)
      description: Retrieve a collection of Lists
      operationId: retrieve-a-collection-of-lists
      x-api-path-slug: lists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Collection
      - Of
      - Lists
      - (latest
      - Version
      - Of
      - Each
      - List)
  /lists/{id}:
    get:
      summary: Retrieve list's latest version
      description: Retrieve latest version of List with specified identifier string
      operationId: retrieve-latest-version-of-list-with-specified-identifier-string
      x-api-path-slug: listsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Lists
      - Latest
      - Version
  /lists/{id}/{version}:
    get:
      summary: Retrieve List's exact version
      description: ""
      operationId: ""
      x-api-path-slug: listsidversion-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Lists
      - Exact
      - Version
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