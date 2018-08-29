{
  "info": {
    "name": "AWS Elastic Beanstalk API Describe Application Versions",
    "_postman_id": "24b794ba-40ed-44e0-8fe8-e7398ce66ed1",
    "description": "Retrieve a list of application versions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Environments",
      "item": [
        {
          "id": "84926dfa-fb46-43ad-bbd4-d66bf294b2ef",
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
              "id": "9ae2b7be-4cce-44c8-b9e0-6062760099f8"
            }
          ]
        },
        {
          "id": "9b2eedd1-48e4-43ed-b4c9-4efc6ae07be4",
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
              "id": "3890f482-05ed-435a-ae1b-e7812915546e"
            }
          ]
        },
        {
          "id": "19d262ce-538a-44fd-9859-77327ec0efe9",
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
              "id": "fd00a9b5-356a-4c14-8174-be286d160072"
            }
          ]
        },
        {
          "id": "394e37e9-a026-49f3-a978-9ffe14d75293",
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
              "id": "8da841eb-6a25-4f10-a126-9b343e75342e"
            }
          ]
        },
        {
          "id": "c8a30346-3844-4105-a39d-e32748a58357",
          "name": "deleteEnvironmentConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEnvironmentConfiguration?ApplicationName=ApplicationName&EnvironmentName=EnvironmentName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the draft configuration associated with the running environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f1ad91d-adf5-4048-bec2-ac60255ceffb"
            }
          ]
        }
      ]
    },
    {
      "name": "DNS",
      "item": [
        {
          "id": "7265e935-1cfd-40ff-b9c2-d285289c5f24",
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
              "id": "fa4f75ba-d78f-432f-bc26-f9d46b179c41"
            }
          ]
        }
      ]
    },
    {
      "name": "Applications",
      "item": [
        {
          "id": "d06bee9f-644e-45a9-ba0c-1b0e9736fee0",
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
              "id": "4ce79a2d-24d1-4c75-8e8b-4b45a4fe3919"
            }
          ]
        },
        {
          "id": "628b6123-f523-4e94-b96a-b7841fb6c333",
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
              "id": "09251b28-0ae3-4ece-983a-ce4d159d0030"
            }
          ]
        },
        {
          "id": "cc1c7a82-de5f-4c90-8561-eb29e17ff101",
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
              "id": "32bc74c8-1741-4052-90ae-de02ce8ba97c"
            }
          ]
        },
        {
          "id": "f046ecd9-874d-44c3-b240-fec01e3d68ea",
          "name": "describeApplications",
          "request": {
            "url": "http://example.com/api/?Action=DescribeApplications?ApplicationNames.member.N=ApplicationNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the descriptions of existing applications."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a09ae87-38ea-4cf8-982d-e8c161f7499e"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Templates",
      "item": [
        {
          "id": "51f58610-5f99-42d3-943b-cfae23757096",
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
              "id": "8bb2f1f3-d8f1-4d3b-8cfb-e6a43ebd5b2f"
            }
          ]
        },
        {
          "id": "a781b232-d772-49ab-b698-e194354807db",
          "name": "deleteConfigurationTemplate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationTemplate?ApplicationName=ApplicationName&TemplateName=TemplateName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified configuration template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85466bbd-9d19-4a5e-a8eb-51386701f5ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Storage Location",
      "item": [
        {
          "id": "08539314-bfca-491e-9ade-364386cc5e08",
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
              "id": "f4172694-a817-4626-81ea-566f4ea142f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Application Version",
      "item": [
        {
          "id": "21318c06-a7fe-4343-891b-627ad93ac00e",
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
              "id": "5c7dcc14-bc4a-4ce5-a198-7be8468f2722"
            }
          ]
        },
        {
          "id": "bb3efa86-b70a-4719-9ede-60e09abdd84f",
          "name": "describeApplicationVersions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeApplicationVersions?ApplicationName=ApplicationName&MaxRecords=MaxRecords&NextToken=NextToken&VersionLabels.member.N=VersionLabels.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a list of application versions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f244a0ea-bd10-4ddb-b1f3-5ea0cf1d9eff"
            }
          ]
        }
      ]
    }
  ]
}