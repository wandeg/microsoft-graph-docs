---
title: "Get directoryDefinition"
description: "Read the properties and relationships of a directoryDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get directoryDefinition

Namespace: microsoft.graph

Read the properties and relationships of a [directoryDefinition](../resources/directorydefinition.md) object.

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
GET /directories/{directoriesId}
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
If successful, this method returns a `200 OK` response code and a [directoryDefinition](../resources/directorydefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_directorydefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/directories/{directoriesId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.directoryDefinition",
    "id": "479269ef-69ef-4792-ef69-9247ef699247",
    "discoveryDateTime": "2016-12-31T23:57:06.5468887+03:00",
    "discoverabilities": "String",
    "name": "Name value",
    "objects": [
      {
        "@odata.type": "microsoft.graph.objectDefinition",
        "attributes": [
          {
            "@odata.type": "microsoft.graph.attributeDefinition",
            "anchor": true,
            "apiExpressions": [
              {
                "@odata.type": "microsoft.graph.stringKeyStringValuePair",
                "key": "Key value",
                "value": "Value value"
              }
            ],
            "caseExact": true,
            "defaultValue": "Default Value value",
            "metadata": [
              {
                "@odata.type": "microsoft.graph.metadataEntry"
              }
            ],
            "multivalued": true,
            "mutability": "String",
            "required": true,
            "referencedObjects": [
              {
                "@odata.type": "microsoft.graph.referencedObject",
                "referencedObjectName": "Referenced Object Name value",
                "referencedProperty": "Referenced Property value"
              }
            ],
            "type": "String"
          }
        ],
        "supportedApis": [
          "Supported Apis value"
        ]
      }
    ],
    "readOnly": true,
    "version": "Version value"
  }
}
```

