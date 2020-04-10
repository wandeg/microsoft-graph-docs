---
title: "Get driveItemVersion"
description: "Read properties and relationships of the driveItemVersion object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get driveItemVersion

Namespace: microsoft.graph

Read properties and relationships of the [driveItemVersion](../resources/driveitemversion.md) object.

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
GET /workbooks/{workbooksId}/versions/{driveItemVersionId}
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/versions/{driveItemVersionId}
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
If successful, this method returns a `200 OK` response code and [driveItemVersion](../resources/driveitemversion.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_driveitemversion"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/versions/{driveItemVersionId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItemVersion"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

{
  "value": {
    "@odata.type": "#microsoft.graph.driveItemVersion",
    "id": "00e11678-1678-00e1-7816-e1007816e100",
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
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
    "publication": {
      "@odata.type": "microsoft.graph.publicationFacet",
      "level": "Level value",
      "versionId": "Version Id value"
    },
    "content": "Stream",
    "size": 4
  }
}
```

