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
  /?Action=CreatePolicyVersion:
    get:
      summary: Create Policy Version
      description: Creates a new version of the specified AWS IoT policy.
      operationId: createPolicyVersion
      x-api-path-slug: actioncreatepolicyversion-get
      parameters:
      - in: query
        name: policyDocument
        description: The JSON document that describes the policy
        type: string
      - in: query
        name: policyName
        description: The policy name
        type: string
      - in: query
        name: setAsDefault
        description: Specifies whether the policy version is set as the default
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=DeletePolicyVersion:
    get:
      summary: Delete Policy Version
      description: Deletes the specified version of the specified policy.
      operationId: deletePolicyVersion
      x-api-path-slug: actiondeletepolicyversion-get
      parameters:
      - in: query
        name: policyName
        description: The name of the policy
        type: string
      - in: query
        name: policyVersionId
        description: The policy version ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=GetPolicyVersion:
    get:
      summary: Get Policy Version
      description: Gets information about the specified policy version.
      operationId: getPolicyVersion
      x-api-path-slug: actiongetpolicyversion-get
      parameters:
      - in: query
        name: policyName
        description: The name of the policy
        type: string
      - in: query
        name: policyVersionId
        description: The policy version ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=SetDefaultPolicyVersion:
    get:
      summary: Set Default Policy Version
      description: Sets the specified version of the specified policy as the policy's
        default (operative) version.
      operationId: setDefaultPolicyVersion
      x-api-path-slug: actionsetdefaultpolicyversion-get
      parameters:
      - in: query
        name: policyName
        description: The policy name
        type: string
      - in: query
        name: policyVersionId
        description: The policy version ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies