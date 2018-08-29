---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 0
info:
  title: AWS Elastic Beanstalk API Update Application Version
  version: 1.0.0
  description: Updates the specified application version to have the specified properties.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeApplicationVersions:
    get:
      summary: Describe Application Versions
      description: Retrieve a list of application versions.
      operationId: describeApplicationVersions
      x-api-path-slug: actiondescribeapplicationversions-get
      parameters:
      - in: query
        name: ApplicationName
        description: Specify an application name to show only application versions
          for that      application
        type: string
      - in: query
        name: MaxRecords
        description: Specify a maximum number of application versions to paginate
          in the request
        type: string
      - in: query
        name: NextToken
        description: Specify a next token to retrieve the next page in a paginated
          request
        type: string
      - in: query
        name: VersionLabels.member.N
        description: Specify a version label to show a specific application version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application Version
  /?Action=CreateApplicationVersion:
    get:
      summary: Create Application Version
      description: Creates an application version for the specified application.
      operationId: createApplicationVersion
      x-api-path-slug: actioncreateapplicationversion-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application
        type: string
      - in: query
        name: AutoCreateApplication
        description: Set to true to create an application with the specified name
          if it doesnt      already exist
        type: string
      - in: query
        name: BuildConfiguration
        description: Settings for an AWS CodeBuild build
        type: string
      - in: query
        name: Description
        description: Describes this version
        type: string
      - in: query
        name: Process
        description: Preprocesses and validates the environment manifest and configuration
          files in the      source bundle
        type: string
      - in: query
        name: SourceBuildInformation
        description: Specify a commit in an AWS CodeCommit Git repository to use as
          the source code for the      application version
        type: string
      - in: query
        name: SourceBundle
        description: The Amazon S3 bucket and key that identify the location of the
          source bundle for this      version
        type: string
      - in: query
        name: VersionLabel
        description: A label identifying this version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=DeleteApplicationVersion:
    get:
      summary: Delete Application Version
      description: Deletes the specified version from the specified application.
      operationId: deleteApplicationVersion
      x-api-path-slug: actiondeleteapplicationversion-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application to which the version belongs
        type: string
      - in: query
        name: DeleteSourceBundle
        description: Set to true to delete the source bundle from your storage bucket
        type: string
      - in: query
        name: VersionLabel
        description: The label of the version to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application Version
  /?Action=UpdateApplicationVersion:
    get:
      summary: Update Application Version
      description: Updates the specified application version to have the specified
        properties.
      operationId: updateApplicationVersion
      x-api-path-slug: actionupdateapplicationversion-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application associated with this version
        type: string
      - in: query
        name: Description
        description: A new description for this version
        type: string
      - in: query
        name: VersionLabel
        description: The name of the version to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
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