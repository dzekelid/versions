---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get project versions
  description: |-
    Returns all versions existing in a single project. The response is not paginated. Use [Get project versions paginated](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-project-projectIdOrKey-version-get) if you want to get the versions in a project with pagination.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ project permission.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /content/{id}/version:
    get:
      summary: Get content versions
      description: "Returns the versions for a piece of content in descending order.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to view the content. If the content is a blog post,
        'View' permission \nfor the space is required."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentVersionResource.getContentVersions_get
      x-api-path-slug: contentidversion-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the content
          to expand
      - in: path
        name: id
        description: The ID of the content to be queried for its versions
      - in: query
        name: limit
        description: The maximum number of versions to return per page
      - in: query
        name: start
        description: The starting index of the returned versions
      responses:
        200:
          description: OK
      tags:
      - Content
      - Versions
    post:
      summary: Restore content version
      description: "Restores a historical version to be the latest version. That is,
        a new version \nis created with the content of the historical version.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentVersionResource.restoreContentVersion_post
      x-api-path-slug: contentidversion-post
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the returnedcontent
          to expand
      - in: path
        name: id
        description: The ID of the content for which the history will be restored
      responses:
        200:
          description: OK
      tags:
      - Restore
      - Content
      - Version
  /content/{id}/version/{versionNumber}:
    get:
      summary: Get content version
      description: "Returns a version for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to view the content. If the content is a blog post,
        'View' permission \nfor the space is required."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentVersionResource.getContentVersion_get
      x-api-path-slug: contentidversionversionnumber-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the content
          to expand
      - in: path
        name: id
        description: The ID of the content to be queried for its version
      - in: path
        name: versionNumber
        description: The number of the version to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Content
      - Version
    delete:
      summary: Delete content version
      description: "Delete a historical version. This does not delete the changes
        made to the \ncontent in that version, rather the changes for the deleted
        version are \nrolled up into the next version. Note, you cannot delete the
        current version.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentVersionResource.deleteContentVersion_delet
      x-api-path-slug: contentidversionversionnumber-delete
      parameters:
      - in: path
        name: id
        description: The ID of the content that the version will be deleted from
      - in: path
        name: versionNumber
        description: The number of the version to be deleted
      responses:
        200:
          description: OK
      tags:
      - Content
      - Version
  /api/2/project/{projectIdOrKey}/version:
    get:
      summary: Get project versions paginated
      description: |-
        Returns a [paginated](https://developer.atlassian.com/cloud/jira/platform/rest/#pagination) representation of all versions existing in a single project. See the [Get project versions](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-project-projectIdOrKey-versions-get) resource if you want to get a full list of versions without pagination.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ project permission.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectResource.getProjectVersionsPaginated_get
      x-api-path-slug: api2projectprojectidorkeyversion-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      - in: query
        name: maxResults
        description: The maximum number of versions to return per page
      - in: query
        name: orderBy
        description: '[Order](https://developer'
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      - in: query
        name: query
        description: Filter the results using a literal string
      - in: query
        name: startAt
        description: The starting index of the returned list of versions (page offset)
      - in: query
        name: status
        description: A comma separated string used to filter the results by version
          status
      responses:
        200:
          description: OK
      tags:
      - Project
      - Versions
      - Paginated
  /api/2/project/{projectIdOrKey}/versions:
    get:
      summary: Get project versions
      description: |-
        Returns all versions existing in a single project. The response is not paginated. Use [Get project versions paginated](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-project-projectIdOrKey-version-get) if you want to get the versions in a project with pagination.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ project permission.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectResource.getProjectVersions_get
      x-api-path-slug: api2projectprojectidorkeyversions-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      responses:
        200:
          description: OK
      tags:
      - Project
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