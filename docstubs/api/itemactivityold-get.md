---
title: "Get itemActivityOLD"
description: "Read properties and relationships of the itemActivityOLD object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get itemActivityOLD

Namespace: microsoft.graph

Read properties and relationships of the [itemActivityOLD](../resources/itemactivityold.md) object.

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
GET /drives/{drivesId}/activities/{itemActivityOLDId}
GET /workbooks/{workbooksId}/activities/{itemActivityOLDId}
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}
GET /me/joinedGroups/{groupId}/drive/list/activities/{itemActivityOLDId}
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/activities/{itemActivityOLDId}
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/activities/{itemActivityOLDId}
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
If successful, this method returns a `200 OK` response code and [itemActivityOLD](../resources/itemactivityold.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_itemactivityold"
}
-->
``` http
GET https://graph.microsoft.com/beta/drives/{drivesId}/activities/{itemActivityOLDId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemActivityOLD"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2501

{
  "value": {
    "@odata.type": "#microsoft.graph.itemActivityOLD",
    "id": "0ee61204-1204-0ee6-0412-e60e0412e60e",
    "action": {
      "@odata.type": "microsoft.graph.itemActionSet",
      "comment": {
        "@odata.type": "microsoft.graph.commentAction",
        "isReply": true,
        "parentAuthor": {
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
        "participants": [
          {
            "@odata.type": "microsoft.graph.identitySet"
          }
        ]
      },
      "create": {
        "@odata.type": "microsoft.graph.createAction"
      },
      "delete": {
        "@odata.type": "microsoft.graph.deleteAction",
        "name": "Name value",
        "objectType": "Object Type value"
      },
      "edit": {
        "@odata.type": "microsoft.graph.editAction"
      },
      "mention": {
        "@odata.type": "microsoft.graph.mentionAction",
        "mentionees": [
          {
            "@odata.type": "microsoft.graph.identitySet"
          }
        ]
      },
      "move": {
        "@odata.type": "microsoft.graph.moveAction",
        "from": "From value",
        "to": "To value"
      },
      "rename": {
        "@odata.type": "microsoft.graph.renameAction",
        "newName": "New Name value",
        "oldName": "Old Name value"
      },
      "restore": {
        "@odata.type": "microsoft.graph.restoreAction"
      },
      "share": {
        "@odata.type": "microsoft.graph.shareAction",
        "recipients": [
          {
            "@odata.type": "microsoft.graph.identitySet"
          }
        ]
      },
      "version": {
        "@odata.type": "microsoft.graph.versionAction",
        "newVersion": "New Version value"
      }
    },
    "actor": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "times": {
      "@odata.type": "microsoft.graph.itemActivityTimeSet",
      "lastRecordedDateTime": "2016-12-31T23:58:00.6127776+00:00",
      "observedDateTime": "2017-01-01T00:01:48.6792519+00:00",
      "recordedDateTime": "2017-01-01T00:00:17.9449043+00:00"
    }
  }
}
```

