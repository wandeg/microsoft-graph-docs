---
title: "Get drive"
description: "Read properties and relationships of the drive object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get drive

Namespace: microsoft.graph

Read properties and relationships of the [drive](../resources/drive.md) object.

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
GET /drive
GET /me/drive
GET /drives/{drivesId}
GET /me/drives/{driveId}
GET /users/{usersId}/drive
GET /sites/{sitesId}/drive
GET /groups/{groupsId}/drive
GET /me/joinedGroups/{groupId}/drive
GET /users/{usersId}/drives/{driveId}
GET /sites/{sitesId}/drives/{driveId}
GET /groups/{groupsId}/drives/{driveId}
GET /me/joinedGroups/{groupId}/drive/list/drive
GET /me/joinedGroups/{groupId}/drives/{driveId}
GET /me/joinedGroups/{groupId}/sites/{siteId}/drive
GET /me/joinedGroups/{groupId}/sites/{siteId}/drives/{driveId}
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
If successful, this method returns a `200 OK` response code and [drive](../resources/drive.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_drive"
}
-->
``` http
GET https://graph.microsoft.com/beta/drive
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2094

{
  "value": {
    "@odata.type": "#microsoft.graph.drive",
    "id": "9c6c0a0c-0a0c-9c6c-0c0a-6c9c0c0a6c9c",
    "createdBy": {
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
    "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
    "description": "Description value",
    "eTag": "ETag value",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
    "name": "Name value",
    "parentReference": {
      "@odata.type": "microsoft.graph.itemReference",
      "driveId": "Drive Id value",
      "driveType": "Drive Type value",
      "path": "Path value",
      "shareId": "Share Id value",
      "sharepointIds": {
        "@odata.type": "microsoft.graph.sharepointIds",
        "listId": "List Id value",
        "listItemId": "List Item Id value",
        "listItemUniqueId": "List Item Unique Id value",
        "siteId": "Site Id value",
        "siteUrl": "https://example.com/siteUrl/",
        "tenantId": "Tenant Id value",
        "webId": "Web Id value"
      }
    },
    "webUrl": "https://example.com/webUrl/",
    "driveType": "Drive Type value",
    "owner": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "quota": {
      "@odata.type": "microsoft.graph.quota",
      "deleted": 7,
      "remaining": 9,
      "state": "State value",
      "total": 5,
      "used": 4,
      "storagePlanInformation": {
        "@odata.type": "microsoft.graph.storagePlanInformation",
        "upgradeAvailable": true
      }
    },
    "sharePointIds": {
      "@odata.type": "microsoft.graph.sharepointIds"
    },
    "system": {
      "@odata.type": "microsoft.graph.systemFacet"
    }
  }
}
```

