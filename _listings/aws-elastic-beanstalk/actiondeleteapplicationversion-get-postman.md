{
  "info": {
    "name": "AWS Elastic Beanstalk API Delete Application Version",
    "_postman_id": "1e695f30-4c43-4b55-baf4-ddd9aaa4c813",
    "description": "Deletes the specified version from the specified application.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Environments",
      "item": [
        {
          "id": "81118979-fe2a-41f7-a704-effa1dbddd9f",
          "name": "abortEnvironmentUpdate",
          "request": {
            "url": "http://example.com/api/?Action=AbortEnvironmentUpdate?EnvironmentId=EnvironmentId&EnvironmentName=EnvironmentName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels in-progress environment configuration update or application version\n      deployment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b0cee54-9625-480e-ba0c-7ca774aafd8e"
            }
          ]
        },
        {
          "id": "b359bfeb-1f54-44e5-b549-0c3be86950bd",
          "name": "applyEnvironmentManagedAction",
          "request": {
            "url": "http://example.com/api/?Action=ApplyEnvironmentManagedAction?ActionId=ActionId&EnvironmentId=EnvironmentId&EnvironmentName=EnvironmentName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a scheduled managed action immediately."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91973c82-2027-48d7-963a-120bd6d67860"
            }
          ]
        },
        {
          "id": "c091540e-02a3-4390-a5d6-29e8e5c2ccaa",
          "name": "composeEnvironments",
          "request": {
            "url": "http://example.com/api/?Action=ComposeEnvironments?ApplicationName=ApplicationName&GroupName=GroupName&VersionLabels.member.N=VersionLabels.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create or update a group of environments that each run a separate component of a single\n      application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cee127a0-3278-420a-9029-e27488c68ac3"
            }
          ]
        },
        {
          "id": "11692ff4-da5a-483f-9e59-2161f4439ad7",
          "name": "createEnvironment",
          "request": {
            "url": "http://example.com/api/?Action=CreateEnvironment?ApplicationName=ApplicationName&CNAMEPrefix=CNAMEPrefix&Description=Description&EnvironmentName=EnvironmentName&GroupName=GroupName&OptionSettings.member.N=OptionSettings.member.N&OptionsToRemove.member.N=OptionsToRemove.member.N&SolutionStackName=SolutionStackName&Tags.member.N=Tags.member.N&TemplateName=TemplateName&Tier=Tier&VersionLabel=VersionLabel",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Launches an environment for the specified application using the specified\n      configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d281f8f3-51fd-4e24-8d58-d4a8b0ad2d4d"
            }
          ]
        }
      ]
    },
    {
      "name": "DNS",
      "item": [
        {
          "id": "b719acff-81c8-4b80-bb5c-c33fc35a4388",
          "name": "checkDNSAvailability",
          "request": {
            "url": "http://example.com/api/?Action=CheckDNSAvailability?CNAMEPrefix=CNAMEPrefix",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks if the specified CNAME is available."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92e96938-149d-44bd-9d22-49afe1182f54"
            }
          ]
        }
      ]
    },
    {
      "name": "Applications",
      "item": [
        {
          "id": "abf83348-156d-4e67-b46e-648be4bf0c5b",
          "name": "createApplication",
          "request": {
            "url": "http://example.com/api/?Action=CreateApplication?ApplicationName=ApplicationName&Description=Description&ResourceLifecycleConfig=ResourceLifecycleConfig",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an application that has one configuration template named default\n      and no application versions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "158e1ae8-d025-4eaf-8fcc-5fdde81a04c1"
            }
          ]
        },
        {
          "id": "ff6c358e-e512-46b4-bf06-0acd7d746b62",
          "name": "createApplicationVersion",
          "request": {
            "url": "http://example.com/api/?Action=CreateApplicationVersion?ApplicationName=ApplicationName&AutoCreateApplication=AutoCreateApplication&BuildConfiguration=BuildConfiguration&Description=Description&Process=Process&SourceBuildInformation=SourceBuildInformation&SourceBundle=SourceBundle&VersionLabel=VersionLabel",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an application version for the specified application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff27be75-316c-44da-9454-53df50b72627"
            }
          ]
        },
        {
          "id": "f2aed0aa-e819-48ae-a4c6-8e9da01a79d5",
          "name": "deleteApplication",
          "request": {
            "url": "http://example.com/api/?Action=DeleteApplication?ApplicationName=ApplicationName&TerminateEnvByForce=TerminateEnvByForce",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified application along with all associated versions and\n      configurations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2000221e-00e8-4055-bc02-118394130473"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Templates",
      "item": [
        {
          "id": "86944270-7815-4240-a36d-ba2c7042cc7f",
          "name": "createConfigurationTemplate",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationTemplate?ApplicationName=ApplicationName&Description=Description&EnvironmentId=EnvironmentId&OptionSettings.member.N=OptionSettings.member.N&SolutionStackName=SolutionStackName&SourceConfiguration=SourceConfiguration&TemplateName=TemplateName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0d30072-ded5-44ea-ac7d-94d5a2cb7a18"
            }
          ]
        }
      ]
    },
    {
      "name": "Storage Location",
      "item": [
        {
          "id": "9799e0c3-0af9-46aa-b807-cd89220f280c",
          "name": "createStorageLocation",
          "request": {
            "url": "http://example.com/api/?Action=CreateStorageLocation?S3Bucket=S3Bucket",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the Amazon S3 storage location for the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed7ffbc2-b111-4c23-8a69-768bdad9c0e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Application Version",
      "item": [
        {
          "id": "b8250c80-70f8-4e69-9fbc-a714784543fb",
          "name": "deleteApplicationVersion",
          "request": {
            "url": "http://example.com/api/?Action=DeleteApplicationVersion?ApplicationName=ApplicationName&DeleteSourceBundle=DeleteSourceBundle&VersionLabel=VersionLabel",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified version from the specified application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01a332e2-4b61-4e4a-9efd-51221ed1fd5b"
            }
          ]
        }
      ]
    }
  ]
}