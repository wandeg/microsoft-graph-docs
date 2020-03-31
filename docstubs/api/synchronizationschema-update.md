---
title: "Update synchronizationSchema"
description: "Update the properties of a synchronizationSchema object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update synchronizationSchema

Namespace: microsoft.graph

Update the properties of a [synchronizationSchema](../resources/synchronizationschema.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema
PATCH /applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}/schema
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [synchronizationSchema](../resources/synchronizationschema.md) object.

The following table shows the properties that are required when you create the [synchronizationSchema](../resources/synchronizationschema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|provisioningTaskIdentifier|String||
|synchronizationRules|[synchronizationRule](../resources/synchronizationrule.md) collection||
|version|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [synchronizationSchema](../resources/synchronizationschema.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3177

{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "id": "cb1c260b-260b-cb1c-0b26-1ccb0b261ccb",
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

