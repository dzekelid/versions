---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Set Default Policy Version
  version: 1.0.0
  description: |-
    Sets the specified version of the specified policy as the policy's default (operative)
          version.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListPolicyVersions:
    get:
      summary: List Policy Versions
      description: |-
        Lists information about the versions of the specified managed policy, including the
              version that is currently set as the policy's default version.
      operationId: listPolicyVersions
      x-api-path-slug: actionlistpolicyversions-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy for which you
          want the      versions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policy Versions
  /?Action=SetDefaultPolicyVersion:
    get:
      summary: Set Default Policy Version
      description: |-
        Sets the specified version of the specified policy as the policy's default (operative)
              version.
      operationId: setDefaultPolicyVersion
      x-api-path-slug: actionsetdefaultpolicyversion-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy whose default
          version you want to      set
        type: string
      - in: query
        name: VersionId
        description: The version of the policy to set as the default (operative) version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default Policy Versions
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