---
title: "List directoryDefinitions"
description: "List properties and relationships of the directoryDefinition objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List directoryDefinitions

Namespace: microsoft.graph

List properties and relationships of the [directoryDefinition](../resources/directorydefinition.md) objects.

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
GET /directories
GET /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/directories
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [directoryDefinition](../resources/directorydefinition.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directorydefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/directories
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directorydefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1644

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directoryDefinition",
      "id": "b9b8a889-a889-b9b8-89a8-b8b989a8b8b9",
      "discoveryDateTime": "2017-01-01T00:01:28.4980686+03:00",
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
  ]
}
```

