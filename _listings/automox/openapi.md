swagger: "2.0"
x-collection-name: Automox
x-complete: 1
info:
  title: Automox API
  description: the-automox-api-is-a-powerful-interface-that-allows-you-to-integrate-automox-reporting-data-into-you-applications-and-control-the-various-settings-of-your-account-all-endpoints-are-only-accessible-via-https-and-are-located-atapi-automox-com--for-instance-you-can-see-events-associated-with-your-account-by-accessing-the-following-url-with-your-idreplace-apikey-with-your-own--httpsconsole-automox-comapieventsapi-keyapikey-limitsbe-nice--if-youre-sending-too-many-requests-too-quickly-well-send-back-a429-error-code-too-many-requests-you-are-limited-to-5000-requests-per-hour-per-api-key-overall--practically-this-means-you-should-when-possible-authenticateusers-so-that-limits-are-well-outside-the-reach-of-a-given-user-
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