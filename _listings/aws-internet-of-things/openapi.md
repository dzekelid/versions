---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
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
      description: Lists the versions of the specified policy and identifies the default
        version.
      operationId: listPolicyVersions
      x-api-path-slug: actionlistpolicyversions-get
      parameters:
      - in: query
        name: policyName
        description: The policy name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policy Versions
---