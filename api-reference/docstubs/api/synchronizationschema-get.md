---
title: "Get synchronizationSchema"
description: "Read the properties and relationships of a synchronizationSchema object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get synchronizationSchema

Namespace: microsoft.graph

Read the properties and relationships of a [synchronizationSchema](../resources/synchronizationschema.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema
GET /applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}/schema
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronizationschema.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.synchronizationSchema",
    "id": "fbd04aeb-4aeb-fbd0-eb4a-d0fbeb4ad0fb",
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
}
```

