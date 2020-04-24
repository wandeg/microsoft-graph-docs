---
title: "Update directoryDefinition"
description: "Update the properties of a directoryDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update directoryDefinition

Namespace: microsoft.graph

Update the properties of a [directoryDefinition](../resources/directorydefinition.md) object.

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
PATCH /directories/{directoriesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [directoryDefinition](../resources/directorydefinition.md) object.

The following table shows the properties that are required when you create the [directoryDefinition](../resources/directorydefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|discoveryDateTime|DateTimeOffset|**TODO: Add Description**|
|discoverabilities|directoryDefinitionDiscoverabilities|**TODO: Add Description**. Possible values are: `None`, `AttributeNames`, `AttributeDataTypes`, `AttributeReadOnly`, `ReferenceAttributes`, `UnknownFutureValue`.|
|name|String|**TODO: Add Description**|
|objects|[objectDefinition](../resources/objectdefinition.md) collection|**TODO: Add Description**|
|readOnly|Boolean|**TODO: Add Description**|
|version|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [directoryDefinition](../resources/directorydefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_directorydefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directories/{directoriesId}
Content-Type: application/json
Content-length: 1378

{
  "@odata.type": "#microsoft.graph.directoryDefinition",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
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
```

