---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get version's related issues count
  description: |-
    Returns the following counts for a version:

    *   Number of issues where the `fixVersion` is set to the version.
    *   Number of issues where the `affectedVersion` is set to the version.
    *   Number of issues where a version custom field is set to the version.

    [Permissions](https://confluence.atlassian.com/x/FQiiLQ) required: _Browse projects_ project permission
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
  /api/2/version/{id}/mergeto/{moveIssuesTo}:
    put:
      summary: Merge versions
      description: Merges two project versions. The merge is completed by deleting
        the version specified in `id` and replacing any occurrences of its ID in `fixVersion`
        with the version ID specified in `moveIssuesTo`. Consider using [Delete and
        replace version](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-version-id-removeAndSwap-post)
        instead. This resource supports swapping version values in `fixVersion`, `affectedVersion`,
        and custom fields. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
        or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.mergeVersions_put
      x-api-path-slug: api2versionidmergetomoveissuesto-put
      parameters:
      - in: path
        name: id
        description: The ID of the version to delete
      - in: path
        name: moveIssuesTo
        description: The ID of the version to merge into
      responses:
        200:
          description: OK
      tags:
      - Merge
      - Versions
  /api/2/version/{id}/relatedIssueCounts:
    get:
      summary: Get version's related issues count
      description: |-
        Returns the following counts for a version:

        *   Number of issues where the `fixVersion` is set to the version.
        *   Number of issues where the `affectedVersion` is set to the version.
        *   Number of issues where a version custom field is set to the version.

        [Permissions](https://confluence.atlassian.com/x/FQiiLQ) required: _Browse projects_ project permission
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getVersionRelatedIssues_get
      x-api-path-slug: api2versionidrelatedissuecounts-get
      parameters:
      - in: path
        name: id
        description: The ID of the version
      responses:
        200:
          description: OK
      tags:
      - Versions
      - Related
      - Issues
      - Count
  /api/2/version/{id}/unresolvedIssueCount:
    get:
      summary: Get version's unresolved issues count
      description: 'Returns counts of the issues and unresolved issues for the project
        version. [Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:
        _Browse projects_ project permission'
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getVersionUnresolvedIssues_get
      x-api-path-slug: api2versionidunresolvedissuecount-get
      parameters:
      - in: path
        name: id
        description: The ID of the version
      responses:
        200:
          description: OK
      tags:
      - Versions
      - Unresolved
      - Issues
      - Count
  /api/2/version:
    post:
      summary: Create version
      description: Creates a project version. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
        or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.createVersion_post
      x-api-path-slug: api2version-post
      responses:
        200:
          description: OK
      tags:
      - Version
  /api/2/version/remotelink:
    get:
      summary: Get remote version links
      description: Returns the remote version links for a given global ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getRemoteVersionLinks_get
      x-api-path-slug: api2versionremotelink-get
      parameters:
      - in: query
        name: globalId
        description: the global ID of the remote resource that is linked to the versions
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Links
  /api/2/version/{id}:
    get:
      summary: Get version
      description: 'Returns a project version. [Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required: _Browse projects_ project permission'
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getVersion_get
      x-api-path-slug: api2versionid-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      - in: path
        name: id
        description: The ID of the version
      responses:
        200:
          description: OK
      tags:
      - Version
    put:
      summary: Update version
      description: Modifies a project version. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
        or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.updateVersion_put
      x-api-path-slug: api2versionid-put
      parameters:
      - in: path
        name: id
        description: The ID of the version
      responses:
        200:
          description: OK
      tags:
      - Version
    delete:
      summary: Delete version
      description: Deletes a project version. Deprecated, use [Delete and replace
        version](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-version-id-removeAndSwap-post)
        that supports swapping version values in custom fields, in addition to the
        swapping for `fixVersion` and `affectedVersion` provided in this resource.
        Alternative versions can be provided to update issues that use the deleted
        version in `fixVersion` or `affectedVersion`. If alternatives are not provided,
        occurrences of `fixVersion` and `affectedVersion` that contain the deleted
        version are cleared. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
        or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.deleteVersion_delete
      x-api-path-slug: api2versionid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the version
      - in: query
        name: moveAffectedIssuesTo
        description: The ID of the version to update `affectedVersion` to when the
          field contains the deleted version
      - in: query
        name: moveFixIssuesTo
        description: The ID of the version to update `fixVersion` to when the field
          contains the deleted version
      responses:
        200:
          description: OK
      tags:
      - Version
  /api/2/version/{id}/move:
    post:
      summary: Move version
      description: Modifies the version's sequence within the project, which affects
        the display order of the versions in Jira. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
        or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.moveVersion_post
      x-api-path-slug: api2versionidmove-post
      parameters:
      - in: path
        name: id
        description: The ID of the version to be moved
      responses:
        200:
          description: OK
      tags:
      - Move
      - Version
  /api/2/version/{id}/removeAndSwap:
    post:
      summary: Delete and replace version
      description: Deletes a project version. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
        or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
        Alternative versions can be provided to update issues that use the deleted
        version in `fixVersion`, `affectedVersion`, or any version picker custom fields.
        If alternatives are not provided, occurrences of `fixVersion`, `affectedVersion`,
        and any version picker custom field, that contain the deleted version, are
        cleared. Any replacement version must be in the same project as the version
        being deleted and cannot be the version being deleted.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.deleteAndReplaceVersion_post
      x-api-path-slug: api2versionidremoveandswap-post
      parameters:
      - in: path
        name: id
        description: The ID of the version
      responses:
        200:
          description: OK
      tags:
      - Replace
      - Version
  /api/2/version/{versionId}/remotelink:
    get:
      summary: Get remote version links by version id
      description: Returns the remote version links associated with the given version
        ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getRemoteVersionLinksByVersionId_get
      x-api-path-slug: api2versionversionidremotelink-get
      parameters:
      - in: path
        name: versionId
        description: a String containing the version ID
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Links
      - By
      - Version
      - Id
    post:
      summary: Create or update remote version link
      description: Create a remote version link via POST. The link's global ID will
        be taken from the JSON payload if provided; otherwise, it will be generated.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.createOrUpdateRemoteVersionLink_post
      x-api-path-slug: api2versionversionidremotelink-post
      parameters:
      - in: path
        name: versionId
      responses:
        200:
          description: OK
      tags:
      - Update
      - Remote
      - Version
      - Link
    delete:
      summary: Delete remote version links by version id
      description: Delete all remote version links for a given version ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.deleteRemoteVersionLinksByVersionId_delete
      x-api-path-slug: api2versionversionidremotelink-delete
      parameters:
      - in: path
        name: versionId
        description: The version for which to delete ALL existing remote version links
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Links
      - By
      - Version
      - Id
  /api/2/version/{versionId}/remotelink/{globalId}:
    get:
      summary: Get remote version link
      description: A REST sub-resource representing a remote version link
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getRemoteVersionLink_get
      x-api-path-slug: api2versionversionidremotelinkglobalid-get
      parameters:
      - in: path
        name: globalId
        description: The id of the remote issue link to be returned
      - in: path
        name: versionId
        description: a String containing the version id
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Link
    post:
      summary: Create or update remote version link with global id
      description: Create a remote version link via POST using the provided global
        ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.createOrUpdateRemoteVersionLinkWithGlobalId_post
      x-api-path-slug: api2versionversionidremotelinkglobalid-post
      parameters:
      - in: path
        name: globalId
      - in: path
        name: versionId
      responses:
        200:
          description: OK
      tags:
      - Update
      - Remote
      - Version
      - Link
      - Global
      - Id
    delete:
      summary: Delete remote version link
      description: Delete a specific remote version link with the given version ID
        and global ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.deleteRemoteVersionLink_delete
      x-api-path-slug: api2versionversionidremotelinkglobalid-delete
      parameters:
      - in: path
        name: globalId
        description: The global ID of the remote link
      - in: path
        name: versionId
        description: The version ID of the remote link
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Link
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