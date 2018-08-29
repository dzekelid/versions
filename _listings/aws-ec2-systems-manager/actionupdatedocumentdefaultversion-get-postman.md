{
  "info": {
    "name": "Amazon EC2 Systems Manager API Update Document Default Version",
    "_postman_id": "a285e371-fcbe-4fb5-a474-ed3df166bc15",
    "description": "Set the default version of a document.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "53be75a3-8432-4454-b1c9-28beecd64116",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&ResourceType=ResourceType&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db355a21-91f3-466d-b2c8-43556448b1e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "b5c83717-a765-4b59-ab39-f4ad8ddd2a8b",
          "name": "cancelCommand",
          "request": {
            "url": "http://example.com/api/?Action=CancelCommand?CommandId=CommandId&InstanceIds=InstanceIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attempts to cancel the command specified by the Command ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "566ddaf6-38b2-430f-98b8-1260a7e9f2f0"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "416a20f9-c659-414f-8a37-e872a709ab70",
          "name": "createActivation",
          "request": {
            "url": "http://example.com/api/?Action=CreateActivation?DefaultInstanceName=DefaultInstanceName&Description=Description&ExpirationDate=ExpirationDate&IamRole=IamRole&RegistrationLimit=RegistrationLimit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers your on-premises server or virtual machine with Amazon EC2 so that you can manage\n   these resources using Run Command."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f18c711-636c-409f-8d00-ef33db5f8aac"
            }
          ]
        },
        {
          "id": "c18f63b2-c0c4-41cf-a031-bd0db4ba8878",
          "name": "deleteActivation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteActivation?ActivationId=ActivationId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an activation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e516c22a-47e7-4814-a033-35bbb7cbc393"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "0f72ff08-f63a-4376-9906-0915e295a9f1",
          "name": "createAssociation",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociation?DocumentVersion=DocumentVersion&InstanceId=InstanceId&Name=Name&OutputLocation=OutputLocation&Parameters=Parameters&ScheduleExpression=ScheduleExpression&Targets=Targets",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75d12adf-03a1-432f-ad10-36fa398c88d7"
            }
          ]
        },
        {
          "id": "91528f3e-1143-4a21-8d07-9be22f42bdbc",
          "name": "createAssociationBatch",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociationBatch?Entries=Entries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94e8d106-6454-4210-aacb-aaaba647348c"
            }
          ]
        },
        {
          "id": "6727b89d-b050-45dc-a768-2c4cf06da5fc",
          "name": "deleteAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates the specified SSM document from the specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38cae666-d04b-4fef-bc29-fb569537f099"
            }
          ]
        },
        {
          "id": "8e1dad6f-b7b5-4ea2-a961-acd78d6a46b9",
          "name": "describeAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the associations for the specified SSM document or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1cac89bc-421d-460f-89a9-b5003314ee20"
            }
          ]
        },
        {
          "id": "b57a8c58-e615-4211-b3e5-7e4bd697cd2d",
          "name": "updateAssociation",
          "request": {
            "url": "http://example.com/api/?Action=UpdateAssociation?AssociationId=AssociationId&DocumentVersion=DocumentVersion&OutputLocation=OutputLocation&Parameters=Parameters&ScheduleExpression=ScheduleExpression",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an association."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f11a5985-9d3d-49a5-b8f7-9515f1054861"
            }
          ]
        },
        {
          "id": "6ea8b1a5-cbba-435f-92d8-07c63d474ab2",
          "name": "updateAssociationStatus",
          "request": {
            "url": "http://example.com/api/?Action=UpdateAssociationStatus?AssociationStatus=AssociationStatus&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the status of the SSM document associated with the specified\n   instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24d77309-cc3d-4e08-a966-ee44dd19ee1c"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "31471331-d3c5-4b34-b6c8-14eec6a8aa9d",
          "name": "createDocument",
          "request": {
            "url": "http://example.com/api/?Action=CreateDocument?Content=Content&DocumentType=DocumentType&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b53ab4ef-d19f-4ad6-8949-f88791bb4321"
            }
          ]
        },
        {
          "id": "f13176a1-fc10-4cc2-8763-fe073493c9d7",
          "name": "deleteDocument",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDocument?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the SSM document and all instance associations to the document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a857bdba-a709-412c-a510-a24f57d8b738"
            }
          ]
        },
        {
          "id": "067ea343-2cb7-402e-9a47-b1aa99a8cb5f",
          "name": "describeDocument",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d2f95f7-aa27-4494-b40c-6756d4814d6f"
            }
          ]
        },
        {
          "id": "f26d470d-16ef-4c60-8c05-c49084ecd3d7",
          "name": "describeDocumentPermission",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocumentPermission?Name=Name&PermissionType=PermissionType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the permissions for an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3429032-cc6c-47bc-bcd4-89503b935868"
            }
          ]
        },
        {
          "id": "486035ff-ee40-49d1-b96b-c437efd44fd5",
          "name": "getDocument",
          "request": {
            "url": "http://example.com/api/?Action=GetDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the contents of the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ef0dc06-94ab-411f-96c9-8f55a17d224b"
            }
          ]
        },
        {
          "id": "087ba78c-611d-435b-8cc4-344f1f345858",
          "name": "updateDocument",
          "request": {
            "url": "http://example.com/api/?Action=UpdateDocument?Content=Content&DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The document you want to update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f775b48-1d28-43e2-85c8-bd0d50f1896f"
            }
          ]
        },
        {
          "id": "99d3aa66-ff40-4e36-a22e-0fd3defd8c48",
          "name": "updateDocumentDefaultVersion",
          "request": {
            "url": "http://example.com/api/?Action=UpdateDocumentDefaultVersion?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Set the default version of a document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "487c3243-9b9c-48d9-b535-fbd2cf87596d"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "c8ef7d93-7932-4fa9-abd5-ee498d23d7fa",
          "name": "createMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=CreateMaintenanceWindow?AllowUnassociatedTargets=AllowUnassociatedTargets&ClientToken=ClientToken&Cutoff=Cutoff&Duration=Duration&Name=Name&Schedule=Schedule",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "113f5c0c-edba-4992-87b7-cbb93e5a92ea"
            }
          ]
        },
        {
          "id": "862deddb-fe1a-4dc7-845e-d1afe6463588",
          "name": "deleteMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeleteMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19fb615e-5f32-4ded-a3a4-ac09c9ba26b0"
            }
          ]
        },
        {
          "id": "97b5f589-e3e2-4165-8f0a-20f83bebef13",
          "name": "describeMaintenanceWindowExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the executions of a Maintenance Window (meaning, information about when the\n   Maintenance Window was scheduled to be active and information about tasks registered and run with\n   the Maintenance Window)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "256bf00c-7d1e-47b1-a7e4-2011654c67dd"
            }
          ]
        },
        {
          "id": "9e689632-932e-4d91-bc47-3cd045bac714",
          "name": "describeMaintenanceWindowExecutionTaskInvocations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTaskInvocations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&TaskId=TaskId&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the individual task executions (one per target) for a particular task executed\n   as part of a Maintenance Window execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f980a3b2-10e3-4938-9c7e-a39b0d87cdd5"
            }
          ]
        },
        {
          "id": "d1f5581c-e142-452e-937a-d0ad932add72",
          "name": "describeMaintenanceWindowExecutionTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "For a given Maintenance Window execution, lists the tasks that were executed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0d2457d-8cdf-4229-8ccc-bcc5c5602f68"
            }
          ]
        },
        {
          "id": "c9f81ff8-cbe7-47b4-98ef-ee7a2d7dd948",
          "name": "describeMaintenanceWindows",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindows?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the Maintenance Windows in an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf4da1d3-555b-482b-b76d-16a6cabd0b9b"
            }
          ]
        },
        {
          "id": "57b4b5b7-0db0-49e2-8ee5-fdf7575c9c32",
          "name": "describeMaintenanceWindowTargets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTargets?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the targets registered with the Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a6fde3f-dd83-455a-b78c-0fa7ce83da00"
            }
          ]
        },
        {
          "id": "dfe5cc24-1377-41a5-b8ff-6b994f5f7feb",
          "name": "describeMaintenanceWindowTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the tasks in a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd9d5a4e-bf87-4a02-98d9-91679287c150"
            }
          ]
        },
        {
          "id": "0830202f-1280-4359-aea7-764b9dff4ddf",
          "name": "getMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8afd730-0579-4528-a4e6-d65d9f65331d"
            }
          ]
        },
        {
          "id": "5e0e794b-5a79-469e-b3bf-6684986e6300",
          "name": "getMaintenanceWindowExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindowExecution?WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves details about a specific task executed as part of a Maintenance Window\n   execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae8c9891-c01e-47e4-bdfa-f9b1e8f380d7"
            }
          ]
        },
        {
          "id": "a9b3a1e1-8fde-4f77-bc17-24d4ab3e01b7",
          "name": "getMaintenanceWindowExecutionTask",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindowExecutionTask?TaskId=TaskId&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the details about a specific task executed as part of a Maintenance Window\n   execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc59c49b-c1f5-492e-8a2c-7d49c2873a4f"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "cf4fd99b-2dbd-412a-ba9f-546a7958742a",
          "name": "createPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePatchBaseline?ApprovalRules=ApprovalRules&ApprovedPatches=ApprovedPatches&ClientToken=ClientToken&Description=Description&GlobalFilters=GlobalFilters&Name=Name&RejectedPatches=RejectedPatches",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ae5dc2f-25cd-4819-b538-8aae004c72e4"
            }
          ]
        },
        {
          "id": "64609e28-081d-4b9a-9198-5d0cf5ca0344",
          "name": "deletePatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae5592e3-efd4-4580-b6bb-0fdcf29d4f27"
            }
          ]
        },
        {
          "id": "728e5eda-affa-406b-89e5-9648200ef1f9",
          "name": "getPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96a45598-9081-4336-bac1-c28029be088e"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter",
      "item": [
        {
          "id": "c95962b6-760a-4c05-a1cb-5c42f345c407",
          "name": "deleteParameter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteParameter?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a parameter from the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5438cab9-a136-4967-8854-eeff6e58288f"
            }
          ]
        },
        {
          "id": "8408ec68-fd2d-42f4-886a-24b17f4236d3",
          "name": "getParameterHistory",
          "request": {
            "url": "http://example.com/api/?Action=GetParameterHistory?MaxResults=MaxResults&Name=Name&NextToken=NextToken&WithDecryption=WithDecryption",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query a list of all parameters used by the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed97ed62-e9c6-419d-b759-3a030d4d387b"
            }
          ]
        },
        {
          "id": "d876cdf7-d550-431c-a44a-a8423b5ae940",
          "name": "putParameter",
          "request": {
            "url": "http://example.com/api/?Action=PutParameter?Description=Description&KeyId=KeyId&Name=Name&Overwrite=Overwrite&Type=Type&Value=Value",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Add one or more paramaters to the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fbf9c38-dc7d-46df-b26a-feb3b5f9e9aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "b00a2edb-61a7-4cb5-bab5-0065de951538",
          "name": "deregisterManagedInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterManagedInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the server or virtual machine from the list of registered servers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45a011a2-8199-4b7b-b1e3-3bd724da5359"
            }
          ]
        },
        {
          "id": "297823ce-c359-4b02-b5e9-d14488df47c7",
          "name": "deregisterPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a patch group from a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4682412-0e2a-4100-91c0-4cae3414d201"
            }
          ]
        },
        {
          "id": "792d09db-47cb-41b0-b93f-5390970b813d",
          "name": "deregisterTargetFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTargetFromMaintenanceWindow?WindowId=WindowId&WindowTargetId=WindowTargetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a target from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd5f7b91-2cbe-4d9b-a672-1d174a89b99f"
            }
          ]
        },
        {
          "id": "f155d534-7d41-4fb3-85b3-c9d6f4056b55",
          "name": "deregisterTaskFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTaskFromMaintenanceWindow?WindowId=WindowId&WindowTaskId=WindowTaskId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a task from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b01460b1-a36c-4d9f-b440-bbfcf70d0491"
            }
          ]
        }
      ]
    },
    {
      "name": "Activations",
      "item": [
        {
          "id": "bffc4786-8ad9-4351-890b-5f8acbb75bb0",
          "name": "describeActivations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActivations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about the activation, including: the date and time the activation was created,\n   the expiration date, the IAM role assigned to the instances in the activation, and the number of\n   instances activated by this registration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e578c95d-dec4-45a4-833b-e01c275ab96a"
            }
          ]
        }
      ]
    },
    {
      "name": "Automation",
      "item": [
        {
          "id": "ba25a93d-85a9-4e91-b7ff-6473d9bf372c",
          "name": "describeAutomationExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutomationExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides details about all active and terminated Automation executions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1b0993f-0073-4f6d-95ce-b14790eb2ec4"
            }
          ]
        },
        {
          "id": "1e129ce8-42ee-4231-b44c-6a7e26e46408",
          "name": "getAutomationExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetAutomationExecution?AutomationExecutionId=AutomationExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get detailed information about a particular Automation execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfd27bed-2473-4e27-9f2f-67296553e5d1"
            }
          ]
        }
      ]
    },
    {
      "name": "Available",
      "item": [
        {
          "id": "2a374264-2539-4f48-a73d-8825f340fc67",
          "name": "describeAvailablePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailablePatches?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patches that could possibly be included in a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "888c9bb3-753e-4d69-ae5d-bca0dbd49b0d"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "b8901ae7-0f97-48c5-8042-38fb63f9e3e0",
          "name": "describeEffectiveInstanceAssociations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectiveInstanceAssociations?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "146ff515-6d2d-4faf-83bc-e8cf0316e396"
            }
          ]
        },
        {
          "id": "57a38c9b-a32b-4ce9-b4e5-b3980c118119",
          "name": "describeEffectivePatchesForPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectivePatchesForPatchBaseline?BaselineId=BaselineId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current effective patches (the patch and the approval state) for the specified patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "106f6597-2f95-4435-a3d6-b5d39339b14b"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "b3b9ad7a-b4cd-4d90-9327-0cb2e3cec11e",
          "name": "describeInstanceAssociationsStatus",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceAssociationsStatus?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The status of the associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "434fd221-9393-40ce-99f6-27441f7ecf54"
            }
          ]
        },
        {
          "id": "a4009b68-c62a-406f-812d-4dc5da838f40",
          "name": "describeInstanceInformation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceInformation?Filters=Filters&InstanceInformationFilterList=InstanceInformationFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92fad724-b622-4134-acb4-79a688e18112"
            }
          ]
        },
        {
          "id": "3a14281b-b2aa-4ad0-9799-6088522e640f",
          "name": "describeInstancePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatches?Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the patches on the specified instance and their state relative to the patch baseline being used for the instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "098f6290-acee-412a-ac0e-d010527d916c"
            }
          ]
        },
        {
          "id": "767bf30d-d443-4c46-834e-ba93da6e45ae",
          "name": "describeInstancePatchStates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStates?InstanceIds=InstanceIds&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state of one or more instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77e6c5a4-06b9-4720-ac2d-3b1b96df4040"
            }
          ]
        },
        {
          "id": "ff752429-9e9b-4e30-986c-d630702eb821",
          "name": "describeInstancePatchStatesForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStatesForPatchGroup?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state for the instances in the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2f638d1-a0a3-4004-8f40-4582dd27da52"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "4d43d794-5d1a-42c7-a41e-bb2cb5e5e560",
          "name": "describeParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeParameters?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3b3ce7e-c61d-4dc0-b314-c1d9a3ca0a6c"
            }
          ]
        },
        {
          "id": "3ef2b2c9-e8e0-4614-a628-a675f8aa3bb6",
          "name": "getParameters",
          "request": {
            "url": "http://example.com/api/?Action=GetParameters?Names=Names&WithDecryption=WithDecryption",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of parameters used by the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0842c87a-126c-4022-a3cc-a2f1ca84b531"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "b771ff43-c075-4db0-a462-c7b37f64570b",
          "name": "describePatchBaselines",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchBaselines?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the patch baselines in your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce979662-c8d1-4cab-8dfd-992b36d0f338"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "1e642b6e-84e7-4c4d-a3f8-2df554abdb17",
          "name": "describePatchGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroups?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patch groups that have been registered with patch baselines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89047cb6-a85c-4aa7-a19f-1fc8cfb54932"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "c4845532-9612-4d04-978b-89ac6114eebf",
          "name": "describePatchGroupState",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroupState?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns high-level aggregated patch compliance state for a patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44cef436-ea5f-4c67-9a21-8adc7fb2df13"
            }
          ]
        }
      ]
    },
    {
      "name": "Command",
      "item": [
        {
          "id": "80f61039-4de7-4d44-9d7d-8294c0051f5a",
          "name": "getCommandInvocation",
          "request": {
            "url": "http://example.com/api/?Action=GetCommandInvocation?CommandId=CommandId&InstanceId=InstanceId&PluginName=PluginName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information about command execution for an invocation or plugin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5b51b7e-9b97-4120-b7c5-c77e63dcdbef"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "1e34bd0b-22d4-4917-9663-7038a3dbb9fc",
          "name": "getDefaultPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetDefaultPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the default patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30c1bc34-7bc3-4a68-a007-469fbade4a63"
            }
          ]
        }
      ]
    },
    {
      "name": "Deployable",
      "item": [
        {
          "id": "571f1bf5-0682-4aad-9317-935b2c490213",
          "name": "getDeployablePatchSnapshotForInstance",
          "request": {
            "url": "http://example.com/api/?Action=GetDeployablePatchSnapshotForInstance?InstanceId=InstanceId&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current snapshot for the patch baseline the instance uses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07ac9452-517b-44f8-be2a-8699d07aeb61"
            }
          ]
        }
      ]
    },
    {
      "name": "Inventory",
      "item": [
        {
          "id": "3b625090-a103-4bf3-b5bb-44b11bd7fd6f",
          "name": "getInventory",
          "request": {
            "url": "http://example.com/api/?Action=GetInventory?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&ResultAttributes=ResultAttributes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query inventory information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52542bbb-5a0b-4cfd-abc1-093a3fc68a52"
            }
          ]
        },
        {
          "id": "e6ea331a-72fe-4c70-afa8-8533799147f2",
          "name": "getInventorySchema",
          "request": {
            "url": "http://example.com/api/?Action=GetInventorySchema?MaxResults=MaxResults&NextToken=NextToken&TypeName=TypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of inventory type names for the account, or return a list of attribute\n   names for a specific Inventory item type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80748025-9fc7-4888-8b51-40e76432fff9"
            }
          ]
        },
        {
          "id": "2840f091-cdaa-492c-a189-edcedf2efdde",
          "name": "putInventory",
          "request": {
            "url": "http://example.com/api/?Action=PutInventory?InstanceId=InstanceId&Items=Items",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Bulk update custom inventory items on one more instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b078a92-f0a1-4464-999f-7cdb7233a275"
            }
          ]
        }
      ]
    },
    {
      "name": "BaselineGroup",
      "item": [
        {
          "id": "1866d6f1-505e-4125-bc83-9419d714fefb",
          "name": "getPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=GetPatchBaselineForPatchGroup?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the patch baseline that should be used for the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec5cddfb-28ae-4243-824a-8a67c260622e"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "6de09852-b251-4962-b247-7da061aedaf8",
          "name": "listAssociations",
          "request": {
            "url": "http://example.com/api/?Action=ListAssociations?AssociationFilterList=AssociationFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the associations for the specified SSM document or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e6171c5-cf9e-4650-810d-78908e8a1c42"
            }
          ]
        },
        {
          "id": "e27fd210-1d09-4acb-86f8-8413b231ef26",
          "name": "listCommandInvocations",
          "request": {
            "url": "http://example.com/api/?Action=ListCommandInvocations?CommandId=CommandId&Details=Details&Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An invocation is copy of a command sent to a specific instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ce68079-6986-468b-a37d-0e7f793462f4"
            }
          ]
        },
        {
          "id": "fd16e276-76f0-44e2-838d-0964a45198fc",
          "name": "listCommands",
          "request": {
            "url": "http://example.com/api/?Action=ListCommands?CommandId=CommandId&Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the commands requested by users of the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e61b7246-8038-42de-b059-d8ad5929963c"
            }
          ]
        },
        {
          "id": "30a09bee-d475-4618-8d78-f77e3a17c06f",
          "name": "listDocuments",
          "request": {
            "url": "http://example.com/api/?Action=ListDocuments?DocumentFilterList=DocumentFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your SSM documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4f78b89-3692-424a-b36f-a525fd2252f6"
            }
          ]
        },
        {
          "id": "14bc6551-01e2-4f5f-bf01-1f7f15671f98",
          "name": "listDocumentVersions",
          "request": {
            "url": "http://example.com/api/?Action=ListDocumentVersions?MaxResults=MaxResults&Name=Name&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all versions for a document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe007ad4-a0d5-4818-b02d-f1cf8e929d38"
            }
          ]
        },
        {
          "id": "d08fb0e0-f375-47d2-8ffe-9ac8ce054785",
          "name": "listInventoryEntries",
          "request": {
            "url": "http://example.com/api/?Action=ListInventoryEntries?Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken&TypeName=TypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of inventory items returned by the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9455da23-efcd-472e-9e51-a0001585ddef"
            }
          ]
        },
        {
          "id": "9057a72a-dafc-404a-bf22-232ccfcc40bd",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?ResourceId=ResourceId&ResourceType=ResourceType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the tags assigned to the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66d01aef-e7a4-4b33-9675-8c7a74c049ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Modify",
      "item": [
        {
          "id": "69ee9171-4114-4607-8b52-b4204d82f39e",
          "name": "modifyDocumentPermission",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDocumentPermission?AccountIdsToAdd=AccountIdsToAdd&AccountIdsToRemove=AccountIdsToRemove&Name=Name&PermissionType=PermissionType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Share a document publicly or privately."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e640746c-b50d-456b-968d-c8f8c1e32635"
            }
          ]
        }
      ]
    },
    {
      "name": "Register",
      "item": [
        {
          "id": "b8ef6a0d-0476-4d4e-9a7e-d5bf03582b5e",
          "name": "registerDefaultPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=RegisterDefaultPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Defines the default patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "479be748-130b-4b30-b5f5-068e4c375957"
            }
          ]
        },
        {
          "id": "a9f58ae5-75b5-4c08-abe2-ed1325d8961d",
          "name": "registerPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=RegisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a patch baseline for a patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61acbcde-2e99-4224-9ab5-cd29491a3e19"
            }
          ]
        },
        {
          "id": "10184760-fd65-48d9-9c02-7ce3e8c0146f",
          "name": "registerTargetWithMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=RegisterTargetWithMaintenanceWindow?ClientToken=ClientToken&OwnerInformation=OwnerInformation&ResourceType=ResourceType&Targets=Targets&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a target with a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5418c5c-e0da-4117-a18e-d2bf7f5ea9b4"
            }
          ]
        },
        {
          "id": "91e14c8a-ae22-4251-87e2-bef1a7e45ae3",
          "name": "registerTaskWithMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=RegisterTaskWithMaintenanceWindow?ClientToken=ClientToken&LoggingInfo=LoggingInfo&MaxConcurrency=MaxConcurrency&MaxErrors=MaxErrors&Priority=Priority&ServiceRoleArn=ServiceRoleArn&Targets=Targets&TaskArn=TaskArn&TaskParameters=TaskParameters&TaskType=TaskType&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new task to a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9589ffac-2cf6-4c8a-99ca-3ae264a373e9"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "9e25a0f8-9de2-4865-9fca-f2f6268aeac7",
          "name": "removeTagsFromResource",
          "request": {
            "url": "http://example.com/api/?Action=RemoveTagsFromResource?ResourceId=ResourceId&ResourceType=ResourceType&TagKeys=TagKeys",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes all tags from the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4338dbf-77d8-4637-a65d-515920aa9433"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "01f6ae8f-8a6f-49be-9645-76ccb158a223",
          "name": "sendCommand",
          "request": {
            "url": "http://example.com/api/?Action=SendCommand?Comment=Comment&DocumentHash=DocumentHash&DocumentHashType=DocumentHashType&DocumentName=DocumentName&InstanceIds=InstanceIds&MaxConcurrency=MaxConcurrency&MaxErrors=MaxErrors&NotificationConfig=NotificationConfig&OutputS3BucketName=OutputS3BucketName&OutputS3KeyPrefix=OutputS3KeyPrefix&OutputS3Region=OutputS3Region&Parameters=Parameters&ServiceRoleArn=ServiceRoleArn&Targets=Targets&TimeoutSeconds=TimeoutSeconds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Executes commands on one or more remote instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aed66a24-efd6-43b3-808d-2ab98d6451d1"
            }
          ]
        }
      ]
    },
    {
      "name": "Start",
      "item": [
        {
          "id": "bb28f473-8c4a-4aa1-8382-6e160fc0fdb4",
          "name": "startAutomationExecution",
          "request": {
            "url": "http://example.com/api/?Action=StartAutomationExecution?DocumentName=DocumentName&DocumentVersion=DocumentVersion&Parameters=Parameters",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates execution of an Automation document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3b846ea-1c5e-477f-a73b-e8f9e340ab80"
            }
          ]
        }
      ]
    },
    {
      "name": "Stop",
      "item": [
        {
          "id": "568965c2-d4a8-48ea-9564-530a67f205ae",
          "name": "stopAutomationExecution",
          "request": {
            "url": "http://example.com/api/?Action=StopAutomationExecution?AutomationExecutionId=AutomationExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stop an Automation that is currently executing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ebb569f-163a-429f-958c-fd1a8b945bb8"
            }
          ]
        }
      ]
    }
  ]
}