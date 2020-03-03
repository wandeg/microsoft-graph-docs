---
title: "List directories"
description: "Get the directoryDefinitions from the directories navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List directories

Get the directoryDefinitions from the directories navigation property.

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
GET /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/directories
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [directoryDefinition](../resources/directorydefinition.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directorydefinition"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/directories
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
      "id": "1be8bff6-bff6-1be8-f6bf-e81bf6bfe81b",
      "discoveryDateTime": "2017-01-01T00:02:10.5924977+03:00",
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

