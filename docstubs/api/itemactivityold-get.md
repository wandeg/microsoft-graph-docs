---
title: "Get itemActivityOLD"
description: "Read properties and relationships of an itemActivityOLD object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get itemActivityOLD

Namespace: microsoft.graph

Read properties and relationships of an [itemActivityOLD](../resources/itemactivityold.md) object.

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
GET /drive/activities/{itemActivityOLDId}
GET /drives/{drivesId}/activities/{itemActivityOLDId}
GET /workbooks/{workbooksId}/activities/{itemActivityOLDId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/list/activities/{itemActivityOLDId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/activities/{itemActivityOLDId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/activities/{itemActivityOLDId}
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
If successful, this method returns a `200 OK` response code and an [itemActivityOLD](../resources/itemactivityold.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_itemactivityold"
}
-->
``` http
GET https://graph.microsoft.com/beta/drive/activities/{itemActivityOLDId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemActivityOLD"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.itemActivityOLD",
    "id": "0d1a0ecf-0ecf-0d1a-cf0e-1a0dcf0e1a0d",
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
      "lastRecordedDateTime": "2016-12-31T23:58:08.649587+03:00",
      "observedDateTime": "2016-12-31T23:56:28.9815191+03:00",
      "recordedDateTime": "2016-12-31T23:58:50.1160597+03:00"
    }
  }
}
```

