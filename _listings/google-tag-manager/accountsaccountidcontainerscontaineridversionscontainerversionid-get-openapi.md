---
swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 0
info:
  title: Google Tag Manager API Get Container Version
  description: Gets a Container Version.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tagmanager/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/containers/{containerId}/versions:
    get:
      summary: Get Container Versions
      description: Lists all Container Versions of a GTM Container.
      operationId: tagmanager.accounts.containers.versions.list
      x-api-path-slug: accountsaccountidcontainerscontaineridversions-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: headers
        description: Retrieve headers only when true
      - in: query
        name: includeDeleted
        description: Also retrieve deleted (archived) versions when true
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
    post:
      summary: Create Container Version
      description: Creates a Container Version.
      operationId: tagmanager.accounts.containers.versions.create
      x-api-path-slug: accountsaccountidcontainerscontaineridversions-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
  /accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}:
    delete:
      summary: Delete Container Version
      description: Deletes a Container Version.
      operationId: tagmanager.accounts.containers.versions.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: containerVersionId
        description: The GTM Container Version ID
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
    get:
      summary: Get Container Version
      description: Gets a Container Version.
      operationId: tagmanager.accounts.containers.versions.get
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: containerVersionId
        description: The GTM Container Version ID
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
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