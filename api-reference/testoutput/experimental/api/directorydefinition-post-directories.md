---
title: "Create directoryDefinition"
description: "Create a new directoryDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create directoryDefinition

Namespace: microsoft.graph

Create a new [directoryDefinition](../resources/directorydefinition.md) object.

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
POST /directories
POST /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/directories
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [directoryDefinition](../resources/directorydefinition.md) object.

The following table shows the properties that are required when you create the [directoryDefinition](../resources/directorydefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|discoveryDateTime|DateTimeOffset||
|discoverabilities|Enumeration|. Possible values are: `None`, `AttributeNames`, `AttributeDataTypes`, `AttributeReadOnly`, `ReferenceAttributes`, `UnknownFutureValue`.|
|name|String||
|objects|[objectDefinition](../resources/objectdefinition.md) collection||
|readOnly|Boolean||
|version|String||



## Response
If successful, this method returns a `201 Created` response code and a [directoryDefinition](../resources/directorydefinition.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_directorydefinition_from_directories"
}
-->
``` http
POST https://graph.microsoft.com/localtest/directories
Content-type: application/json
Content-length: 1378

{
  "@odata.type": "#microsoft.graph.directoryDefinition",
  "discoveryDateTime": "2017-01-01T00:00:15.3514116+03:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorydefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1427

{
  "@odata.type": "#microsoft.graph.directoryDefinition",
  "id": "d9b1804a-804a-d9b1-4a80-b1d94a80b1d9",
  "discoveryDateTime": "2017-01-01T00:00:15.3514116+03:00",
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

