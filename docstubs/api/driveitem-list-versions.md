---
title: "List versions"
description: "Get the driveItemVersions from the versions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List versions

Namespace: microsoft.graph

Get the driveItemVersions from the versions navigation property.

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
GET /workbooks/{workbooksId}/versions
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/versions
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
If successful, this method returns a `200 OK` response code and a collection of [driveItemVersion](../resources/driveitemversion.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_driveitemversion"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/versions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.driveitemversion)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 859

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.driveItemVersion",
      "id": "2ed88826-8826-2ed8-2688-d82e2688d82e",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value",
          "displayName": "Display Name value"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        },
        "user": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
      "publication": {
        "@odata.type": "microsoft.graph.publicationFacet",
        "level": "Level value",
        "versionId": "Version Id value"
      },
      "content": "Stream",
      "size": 4
    }
  ]
}
```

