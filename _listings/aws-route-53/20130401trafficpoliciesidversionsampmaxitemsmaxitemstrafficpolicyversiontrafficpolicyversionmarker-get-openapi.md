---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 0
info:
  title: AWS Route 53 API List Traffic Policy Versions
  version: 1.0.0
  description: 'Gets information about all of the versions for a specified traffic
    policy.Send a GET request to the /Amazon Route 53 APIversion/trafficpolicy resource
    and specify the ID of the traffic policyfor which you want to list versions.Amazon
    Route 53 returns a maximum of 100 items in each response. If you have a lot of
    trafficpolicies, you can use the maxitems parameter to list them in groups of
    up to100.The response includes three values that help you navigate from one group
    ofmaxitems traffic policies to the next:             IsTruncated           If
    the value of IsTruncated in the response is true,there are more traffic policy
    versions associated with the specified trafficpolicy.If IsTruncated is false,
    this response includes the lasttraffic policy version that is associated with
    the specified traffic policy.             TrafficPolicyVersionMarker           The
    ID of the next traffic policy version that is associated with the current AWSaccount.
    If you want to list more traffic policies, make another call toListTrafficPolicyVersions,
    and specify the value of theTrafficPolicyVersionMarker element in theTrafficPolicyVersionMarker
    request parameter.If IsTruncated is false, Amazon Route 53 omits theTrafficPolicyVersionMarker
    element from the response.             MaxItems           The value that you specified
    for the MaxItems parameter in the requestthat produced the current response.'
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/trafficpolicies/Id/versions&amp;maxitems=MaxItems?trafficpolicyversion=TrafficPolicyVersionMarker:
    get:
      summary: List Traffic Policy Versions
      description: 'Gets information about all of the versions for a specified traffic
        policy.Send a GET request to the /Amazon Route 53 APIversion/trafficpolicy
        resource and specify the ID of the traffic policyfor which you want to list
        versions.Amazon Route 53 returns a maximum of 100 items in each response.
        If you have a lot of trafficpolicies, you can use the maxitems parameter to
        list them in groups of up to100.The response includes three values that help
        you navigate from one group ofmaxitems traffic policies to the next:             IsTruncated           If
        the value of IsTruncated in the response is true,there are more traffic policy
        versions associated with the specified trafficpolicy.If IsTruncated is false,
        this response includes the lasttraffic policy version that is associated with
        the specified traffic policy.             TrafficPolicyVersionMarker           The
        ID of the next traffic policy version that is associated with the current
        AWSaccount. If you want to list more traffic policies, make another call toListTrafficPolicyVersions,
        and specify the value of theTrafficPolicyVersionMarker element in theTrafficPolicyVersionMarker
        request parameter.If IsTruncated is false, Amazon Route 53 omits theTrafficPolicyVersionMarker
        element from the response.             MaxItems           The value that you
        specified for the MaxItems parameter in the requestthat produced the current
        response.'
      operationId: listtrafficpolicyversions
      x-api-path-slug: 20130401trafficpoliciesidversionsampmaxitemsmaxitemstrafficpolicyversiontrafficpolicyversionmarker-get
      parameters:
      - in: path
        name: Id
        description: Specify the value of Id of the traffic policy for which you want
          to listall versions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Traffic Policies
  /2013-04-01/trafficpolicy/Id:
    post:
      summary: Create Traffic Policy Version
      description: Creates a new version of an existing traffic policy. When you create
        a new version of atraffic policy, you specify the ID of the traffic policy
        that you want to update and aJSON-formatted document that describes the new
        version. You use traffic policies to createmultiple DNS resource record sets
        for one domain name (such as example.com) or one subdomainname (such as www.example.com).
        You can create a maximum of 1000 versions of a traffic policy.If you reach
        the limit and need to create another version, you'll need to start a new trafficpolicy.Send
        a POST request to the /2013-04-01/trafficpolicy/ resource. The request body
        includes a document witha CreateTrafficPolicyVersionRequest element. The response
        returns theCreateTrafficPolicyVersionResponse element, which contains information
        aboutthe new version of the traffic policy.
      operationId: createtrafficpolicyversion
      x-api-path-slug: 20130401trafficpolicyid-post
      parameters:
      - in: body
        name: Comment
        description: The comment that you specified in the CreateTrafficPolicyVersion
          request,if any
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: CreateTrafficPolicyVersionRequest
        description: Root level tag for the CreateTrafficPolicyVersionRequest parameters
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: Document
        description: The definition of this version of the traffic policy, in JSON
          format
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: Id
        description: The ID of the traffic policy for which you want to create a new
          version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Traffic Policies
  /2013-04-01/trafficpolicy/Id/Version:
    delete:
      summary: Delete Traffic Policy
      description: Deletes a traffic policy.Send a DELETE request to the /Amazon Route
        53 APIversion/trafficpolicy resource.
      operationId: deletetrafficpolicy
      x-api-path-slug: 20130401trafficpolicyidversion-delete
      parameters:
      - in: path
        name: Id
        description: The ID of the traffic policy that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Traffic Policies
    get:
      summary: Get Traffic Policy
      description: Gets information about a specific traffic policy version.Send a
        GET request to the /Amazon Route 53 APIversion/trafficpolicy resource.
      operationId: gettrafficpolicy
      x-api-path-slug: 20130401trafficpolicyidversion-get
      parameters:
      - in: path
        name: Id
        description: The ID of the traffic policy that you want to get information
          about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Traffic Policies
    post:
      summary: Update Traffic Policy Comment
      description: Updates the comment for a specified traffic policy version.Send
        a POST request to the /2013-04-01/trafficpolicy/ resource.The request body
        must include a document with anUpdateTrafficPolicyCommentRequest element.
      operationId: updatetrafficpolicycomment
      x-api-path-slug: 20130401trafficpolicyidversion-post
      parameters:
      - in: body
        name: Comment
        description: The new comment for the specified traffic policy and version
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: Id
        description: The value of Id for the traffic policy for which you want to
          update thecomment
        type: string
      - in: body
        name: UpdateTrafficPolicyCommentRequest
        description: Root level tag for the UpdateTrafficPolicyCommentRequest parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Traffic Policies
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