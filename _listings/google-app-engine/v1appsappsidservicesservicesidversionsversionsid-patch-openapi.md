---
swagger: "2.0"
x-collection-name: Google App Engine
x-complete: 0
info:
  title: Google App Engine Admin API Update Version
  description: 'Updates the specified Version resource. You can specify the following
    fields depending on the App Engine environment and type of scaling that the version
    resource uses: serving_status (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.serving_status):
    For Version resources that use basic scaling, manual scaling, or run in the App
    Engine flexible environment. instance_class (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.instance_class):
    For Version resources that run in the App Engine standard environment. automatic_scaling.min_idle_instances
    (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.automatic_scaling):
    For Version resources that use automatic scaling and run in the App Engine standard
    environment. automatic_scaling.max_idle_instances (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.automatic_scaling):
    For Version resources that use automatic scaling and run in the App Engine standard
    environment.'
  contact:
    name: Google
    url: https://google.com
  version: v1
host: appengine.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/apps/{appsId}/services/{servicesId}/versions:
    get:
      summary: Get Versions
      description: Lists the versions of a service.
      operationId: appengine.apps.services.versions.list
      x-api-path-slug: v1appsappsidservicesservicesidversions-get
      parameters:
      - in: path
        name: appsId
        description: Part of `parent`
      - in: query
        name: pageSize
        description: Maximum results to return per page
      - in: query
        name: pageToken
        description: Continuation token for fetching the next page of results
      - in: path
        name: servicesId
        description: Part of `parent`
      - in: query
        name: view
        description: Controls the set of fields returned in the List response
      responses:
        200:
          description: OK
      tags:
      - Version
    post:
      summary: Deploy Version
      description: Deploys code and resource files to a new version.
      operationId: appengine.apps.services.versions.create
      x-api-path-slug: v1appsappsidservicesservicesidversions-post
      parameters:
      - in: path
        name: appsId
        description: Part of `parent`
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: servicesId
        description: Part of `parent`
      responses:
        200:
          description: OK
      tags:
      - Version
  /v1/apps/{appsId}/services/{servicesId}/versions/{versionsId}:
    delete:
      summary: Delete Version
      description: Deletes an existing Version resource.
      operationId: appengine.apps.services.versions.delete
      x-api-path-slug: v1appsappsidservicesservicesidversionsversionsid-delete
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      - in: path
        name: versionsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Version
    get:
      summary: Get Version
      description: Gets the specified Version resource. By default, only a BASIC_VIEW
        will be returned. Specify the FULL_VIEW parameter to get the full resource.
      operationId: appengine.apps.services.versions.get
      x-api-path-slug: v1appsappsidservicesservicesidversionsversionsid-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      - in: path
        name: versionsId
        description: Part of `name`
      - in: query
        name: view
        description: Controls the set of fields returned in the Get response
      responses:
        200:
          description: OK
      tags:
      - Version
    patch:
      summary: Update Version
      description: 'Updates the specified Version resource. You can specify the following
        fields depending on the App Engine environment and type of scaling that the
        version resource uses: serving_status (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.serving_status):
        For Version resources that use basic scaling, manual scaling, or run in the
        App Engine flexible environment. instance_class (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.instance_class):
        For Version resources that run in the App Engine standard environment. automatic_scaling.min_idle_instances
        (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.automatic_scaling):
        For Version resources that use automatic scaling and run in the App Engine
        standard environment. automatic_scaling.max_idle_instances (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.automatic_scaling):
        For Version resources that use automatic scaling and run in the App Engine
        standard environment.'
      operationId: appengine.apps.services.versions.patch
      x-api-path-slug: v1appsappsidservicesservicesidversionsversionsid-patch
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: servicesId
        description: Part of `name`
      - in: query
        name: updateMask
        description: Standard field mask for the set of fields to be updated
      - in: path
        name: versionsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
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