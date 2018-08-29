{
  "info": {
    "name": "AWS Lambda API Publish Version",
    "_postman_id": "84ec372e-728e-40d3-9f3b-69d753fa36e2",
    "description": "Publishes a version of your function from the current snapshot of $LATEST.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "60df63ff-f442-4866-a9a0-264804cc70d5",
          "name": "addPermission",
          "request": {
            "url": "http://example.com/api/?Action=AddPermission?FunctionName=FunctionName&Qualifier=Qualifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a permission to the resource policy associated with the specified AWS Lambda function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db8e5f95-eef0-41d7-af2f-4fc9a20672e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Aliases",
      "item": [
        {
          "id": "05e870a2-36c4-4dfb-82c6-99292d72115e",
          "name": "createAlias",
          "request": {
            "url": "http://example.com/api/?Action=CreateAlias?FunctionName=FunctionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an alias that points to the specified Lambda function version."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75afd202-bf5e-4b13-b8b3-2a46ff3b91a2"
            }
          ]
        },
        {
          "id": "df802b23-cf8b-4818-8196-0c89499ccb9f",
          "name": "deleteAlias",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAlias?FunctionName=FunctionName&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Lambda function alias."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3156d9e0-bb42-44d8-a0d9-e2bf7c917076"
            }
          ]
        },
        {
          "id": "848d96b4-873d-4f63-8580-e80406e94002",
          "name": "getAlias",
          "request": {
            "url": "http://example.com/api/?Action=GetAlias?FunctionName=FunctionName&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the specified alias information such as the alias ARN, description, and function version it \n      is pointing to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30fd5563-7236-4be2-b774-ad0f144a5989"
            }
          ]
        },
        {
          "id": "fc4ea461-7f33-4725-9657-a6e5ee75d2b9",
          "name": "listAliases",
          "request": {
            "url": "http://example.com/api/?Action=ListAliases?FunctionName=FunctionName&FunctionVersion=FunctionVersion&Marker=Marker&MaxItems=MaxItems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of aliases created for a Lambda function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84ff6e27-0c13-4f46-91b5-eaf7cb5b14a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Sources",
      "item": [
        {
          "id": "5ccc739a-f80c-404b-a658-d2d8905ded4c",
          "name": "createEventSourceMapping",
          "request": {
            "url": "http://example.com/api/?Action=CreateEventSourceMapping?BatchSize=BatchSize&Enabled=Enabled&EventSourceArn=EventSourceArn&FunctionName=FunctionName&StartingPosition=StartingPosition&StartingPositionTimestamp=StartingPositionTimestamp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Identifies a stream as an event source for a Lambda function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "302f0529-61aa-47a4-84f7-4b19b45eaed3"
            }
          ]
        },
        {
          "id": "d360f7b1-f233-4d2c-b995-a297fc5f94d8",
          "name": "deleteEventSourceMapping",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEventSourceMapping?UUID=UUID",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an event source mapping."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21cf6eb4-290c-4cfb-aa8e-aa2b791c467c"
            }
          ]
        },
        {
          "id": "f31394f7-c8d3-4174-b09c-e0ed2d0ef9c0",
          "name": "getEventSourceMapping",
          "request": {
            "url": "http://example.com/api/?Action=GetEventSourceMapping?UUID=UUID",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns configuration information for the specified event source mapping (see."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1db59fb4-c5ff-4c3b-a837-57c8b84ef996"
            }
          ]
        },
        {
          "id": "42b204fa-61a5-4392-9c58-63369b7ffd6b",
          "name": "listEventSourceMappings",
          "request": {
            "url": "http://example.com/api/?Action=ListEventSourceMappings?EventSourceArn=EventSourceArn&FunctionName=FunctionName&Marker=Marker&MaxItems=MaxItems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of event source mappings you created using the CreateEventSourceMapping \n      (see."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d5730ae-d4d7-4e9f-8fb5-973c1a84e092"
            }
          ]
        }
      ]
    },
    {
      "name": "Functions",
      "item": [
        {
          "id": "f33b5fc6-6d7a-4f5a-a235-86f19f067be7",
          "name": "createFunction",
          "request": {
            "url": "http://example.com/api/?Action=CreateFunction?Code=Code&DeadLetterConfig=DeadLetterConfig&Description=Description&Environment=Environment&FunctionName=FunctionName&Handler=Handler&KMSKeyArn=KMSKeyArn&MemorySize=MemorySize&Publish=Publish&Role=Role&Runtime=Runtime&Timeout=Timeout&VpcConfig=VpcConfig",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Lambda function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d73de098-47dc-4d49-a725-9e22e3cee844"
            }
          ]
        },
        {
          "id": "32f5a2ee-a0d4-4959-9c68-5b2495858b8b",
          "name": "deleteFunction",
          "request": {
            "url": "http://example.com/api/?Action=DeleteFunction?FunctionName=FunctionName&Qualifier=Qualifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Lambda function code and configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f68b9eb2-4bb3-4678-a36e-3c4842b36aa3"
            }
          ]
        },
        {
          "id": "04b38743-7e4e-48c2-b400-3f9b40924b28",
          "name": "getFunction",
          "request": {
            "url": "http://example.com/api/?Action=GetFunction?FunctionName=FunctionName&Qualifier=Qualifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the configuration information of the Lambda function and a presigned URL \n      link to the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "969b729a-e4e3-4278-bd92-fc3fca28c7e0"
            }
          ]
        },
        {
          "id": "4c868003-a2ae-4602-a2eb-1ab7289c43c4",
          "name": "getFunctionConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=GetFunctionConfiguration?FunctionName=FunctionName&Qualifier=Qualifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the configuration information of the Lambda function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "499c5ab1-64ab-432d-883e-c2b230232df1"
            }
          ]
        },
        {
          "id": "bf208efc-2052-49cc-95dd-f75760f02565",
          "name": "listFunctions",
          "request": {
            "url": "http://example.com/api/?Action=ListFunctions?Marker=Marker&MaxItems=MaxItems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your Lambda functions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17f2b03c-8f72-4386-b767-bbb875322d3d"
            }
          ]
        },
        {
          "id": "b6e55c0f-aace-49e0-a4f8-d6bc6b8700c6",
          "name": "listVersionsByFunction",
          "request": {
            "url": "http://example.com/api/?Action=ListVersionsByFunction?FunctionName=FunctionName&Marker=Marker&MaxItems=MaxItems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all versions of a function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80ecf9f5-fdf3-4d22-a5ee-9f4a8bad22aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "9c1cf829-cc90-44dd-82fa-7d72f24bc896",
          "name": "getAccountSettings",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountSettings?AccountLimit=AccountLimit&AccountUsage=AccountUsage",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a customer's account settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3644cea-15b6-4899-948b-293760bfe882"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "1da086a2-a258-473e-ac16-114221129c1d",
          "name": "getPolicy",
          "request": {
            "url": "http://example.com/api/?Action=GetPolicy?FunctionName=FunctionName&Qualifier=Qualifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the resource policy associated with the specified Lambda function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92977bc5-bcfa-4b4d-b924-f76c47593025"
            }
          ]
        }
      ]
    },
    {
      "name": "Invoke",
      "item": [
        {
          "id": "5023b7fc-9caa-4ef8-97f1-ff44be037ab2",
          "name": "invoke",
          "request": {
            "url": "http://example.com/api/?Action=Invoke?ClientContext=ClientContext&FunctionName=FunctionName&InvocationType=InvocationType&LogType=LogType&Qualifier=Qualifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Invokes a specific Lambda function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a54b044-e914-45e2-86e8-31820c24b056"
            }
          ]
        }
      ]
    },
    {
      "name": "Async",
      "item": [
        {
          "id": "298c65fe-757d-4e5f-a054-d80f90346be6",
          "name": "invokeAsync",
          "request": {
            "url": "http://example.com/api/?Action=InvokeAsync?FunctionName=FunctionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "ImportantThis API is deprecated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "113d1e65-fa77-4a21-9c88-b7b7ffd69b4d"
            }
          ]
        }
      ]
    },
    {
      "name": "Version",
      "item": [
        {
          "id": "ab478896-6e04-45f0-9e3a-171d9649785a",
          "name": "publishVersion",
          "request": {
            "url": "http://example.com/api/?Action=PublishVersion?FunctionName=FunctionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Publishes a version of your function from the current snapshot of $LATEST."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c66db83e-4843-4475-b650-9dc5bd428579"
            }
          ]
        }
      ]
    }
  ]
}