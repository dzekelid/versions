---
swagger: "2.0"
x-collection-name: Automox
x-complete: 0
info:
  title: Automox Get Software Version
  description: Retrieves software packages and patches for an organization, specific
    policy, or just those that need [approval | attention | exceptions | pending update].
  termsOfService: https://www.automox.com/
  contact:
    name: support@automox.com
  version: 1.0.0
host: console.automox.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /software_version:
    get:
      summary: Get Software Version
      description: Retrieves software packages and patches for an organization, specific
        policy, or just those that need [approval | attention | exceptions | pending
        update].
      operationId: retrieves-software-packages-and-patches-for-an-organization-specific-policy-or-just-those-that-need-
      x-api-path-slug: software-version-get
      parameters:
      - in: query
        name: exceptions
        description: Retrieve software that applies to exception endpoints
      - in: query
        name: l
        description: Result Limit
      - in: query
        name: needsApproval
        description: Retrieve software that needs approval
      - in: query
        name: needsAttention
        description: Retrieve software that needs attention
      - in: query
        name: o
        description: Organization ID
      - in: query
        name: p
        description: Page Number
      - in: query
        name: pendingUpdate
        description: Retrieve software that is pending update
      - in: query
        name: policyId
        description: Return results for a specific Policy ID
      responses:
        200:
          description: OK
      tags:
      - Software
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