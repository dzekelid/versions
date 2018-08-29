swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeConversionTasks:
    get:
      summary: Describe Conversion Tasks
      description: Describes one or more of your conversion tasks.
      operationId: describeconversiontasks
      x-api-path-slug: actiondescribeconversiontasks-get
      responses:
        200:
          description: OK
      tags:
      - Version Tasks