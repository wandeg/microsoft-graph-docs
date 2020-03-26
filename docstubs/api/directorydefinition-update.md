---
title: "Update directoryDefinition"
description: "Update the properties of a directoryDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update directoryDefinition

Namespace: microsoft.graph

Update the properties of a [directoryDefinition](../resources/directorydefinition.md) object.

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
PATCH /directories/{directoriesId}
PATCH /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/directories/{directoryDefinitionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [directoryDefinition](../resources/directorydefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_directorydefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directories/{directoriesId}
Content-type: application/json
Content-length: 1378

{
  "@odata.type": "#microsoft.graph.directoryDefinition",
  "discoveryDateTime": "2016-12-31T23:59:39.2125155+00:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1427

{
  "@odata.type": "#microsoft.graph.directoryDefinition",
  "id": "4b7f7194-7194-4b7f-9471-7f4b94717f4b",
  "discoveryDateTime": "2016-12-31T23:59:39.2125155+00:00",
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

