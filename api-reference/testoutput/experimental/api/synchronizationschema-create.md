---
title: "Create synchronizationSchema"
description: "Create a new synchronizationSchema object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create synchronizationSchema

Create a new [synchronizationSchema](../resources/synchronizationschema.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.synchronizationSchema not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the synchronizationSchema object.

The following table shows the properties that are required when you create the synchronizationSchema.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|provisioningTaskIdentifier|String||
|synchronizationRules|[synchronizationRule](../resources/synchronizationRule.md) collection||
|version|String||



## Response
If successful, this method returns a `201 Created` response code and a [synchronizationSchema](../resources/synchronizationschema.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_synchronizationschema_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.synchronizationSchema not found
Content-type: application/json
Content-length: 3128

{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "provisioningTaskIdentifier": "Provisioning Task Identifier value",
  "synchronizationRules": [
    {
      "@odata.type": "microsoft.graph.synchronizationRule",
      "editable": true,
      "id": "Id value",
      "metadata": [
        {
          "@odata.type": "microsoft.graph.stringKeyStringValuePair",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "name": "Name value",
      "objectMappings": [
        {
          "@odata.type": "microsoft.graph.objectMapping",
          "attributeMappings": [
            {
              "@odata.type": "microsoft.graph.attributeMapping",
              "defaultValue": "Default Value value",
              "exportMissingReferences": true,
              "flowBehavior": "String",
              "flowType": "String",
              "matchingPriority": 0,
              "source": {
                "@odata.type": "microsoft.graph.attributeMappingSource",
                "expression": "Expression value",
                "parameters": [
                  {
                    "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair",
                    "value": {
                      "@odata.type": "microsoft.graph.attributeMappingSource",
                      "type": "String"
                    }
                  }
                ]
              },
              "targetAttributeName": "Target Attribute Name value"
            }
          ],
          "enabled": true,
          "flowTypes": "String",
          "metadata": [
            {
              "@odata.type": "microsoft.graph.metadataEntry"
            }
          ],
          "scope": {
            "@odata.type": "microsoft.graph.filter",
            "groups": [
              {
                "@odata.type": "microsoft.graph.filterGroup",
                "clauses": [
                  {
                    "@odata.type": "microsoft.graph.filterClause",
                    "operatorName": "Operator Name value",
                    "sourceOperandName": "Source Operand Name value",
                    "targetOperand": {
                      "@odata.type": "microsoft.graph.filterOperand",
                      "values": [
                        "Values value"
                      ]
                    }
                  }
                ]
              }
            ],
            "inputFilterGroups": [
              {
                "@odata.type": "microsoft.graph.filterGroup"
              }
            ],
            "categoryFilterGroups": [
              {
                "@odata.type": "microsoft.graph.filterGroup"
              }
            ]
          },
          "sourceObjectName": "Source Object Name value",
          "targetObjectName": "Target Object Name value"
        }
      ],
      "priority": 8,
      "sourceDirectoryName": "Source Directory Name value",
      "targetDirectoryName": "Target Directory Name value"
    }
  ],
  "version": "Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationschema"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3177

{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "id": "384985da-85da-3849-da85-4938da854938",
  "provisioningTaskIdentifier": "Provisioning Task Identifier value",
  "synchronizationRules": [
    {
      "@odata.type": "microsoft.graph.synchronizationRule",
      "editable": true,
      "id": "Id value",
      "metadata": [
        {
          "@odata.type": "microsoft.graph.stringKeyStringValuePair",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "name": "Name value",
      "objectMappings": [
        {
          "@odata.type": "microsoft.graph.objectMapping",
          "attributeMappings": [
            {
              "@odata.type": "microsoft.graph.attributeMapping",
              "defaultValue": "Default Value value",
              "exportMissingReferences": true,
              "flowBehavior": "String",
              "flowType": "String",
              "matchingPriority": 0,
              "source": {
                "@odata.type": "microsoft.graph.attributeMappingSource",
                "expression": "Expression value",
                "parameters": [
                  {
                    "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair",
                    "value": {
                      "@odata.type": "microsoft.graph.attributeMappingSource",
                      "type": "String"
                    }
                  }
                ]
              },
              "targetAttributeName": "Target Attribute Name value"
            }
          ],
          "enabled": true,
          "flowTypes": "String",
          "metadata": [
            {
              "@odata.type": "microsoft.graph.metadataEntry"
            }
          ],
          "scope": {
            "@odata.type": "microsoft.graph.filter",
            "groups": [
              {
                "@odata.type": "microsoft.graph.filterGroup",
                "clauses": [
                  {
                    "@odata.type": "microsoft.graph.filterClause",
                    "operatorName": "Operator Name value",
                    "sourceOperandName": "Source Operand Name value",
                    "targetOperand": {
                      "@odata.type": "microsoft.graph.filterOperand",
                      "values": [
                        "Values value"
                      ]
                    }
                  }
                ]
              }
            ],
            "inputFilterGroups": [
              {
                "@odata.type": "microsoft.graph.filterGroup"
              }
            ],
            "categoryFilterGroups": [
              {
                "@odata.type": "microsoft.graph.filterGroup"
              }
            ]
          },
          "sourceObjectName": "Source Object Name value",
          "targetObjectName": "Target Object Name value"
        }
      ],
      "priority": 8,
      "sourceDirectoryName": "Source Directory Name value",
      "targetDirectoryName": "Target Directory Name value"
    }
  ],
  "version": "Version value"
}
```

