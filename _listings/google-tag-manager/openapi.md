swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 1
info:
  title: Tag Manager
  description: accesses-tag-manager-accounts-and-containers-
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
    put:
      summary: Update Container Version
      description: Updates a Container Version.
      operationId: tagmanager.accounts.containers.versions.update
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionid-put
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
      - in: path
        name: containerVersionId
        description: The GTM Container Version ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the container version in storage
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
  /accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/publish:
    post:
      summary: Publish Container Version
      description: Publishes a Container Version.
      operationId: tagmanager.accounts.containers.versions.publish
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionidpublish-post
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
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the container version in storage
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
  /accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/restore:
    post:
      summary: Restore Container Version
      description: Restores a Container Version. This will overwrite the container's
        current configuration (including its variables, triggers and tags). The operation
        will not have any effect on the version that is being served (i.e. the published
        version).
      operationId: tagmanager.accounts.containers.versions.restore
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionidrestore-post
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
  /accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/undelete:
    post:
      summary: Undelete Container Version
      description: Undeletes a Container Version.
      operationId: tagmanager.accounts.containers.versions.undelete
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionidundelete-post
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