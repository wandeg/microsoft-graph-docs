---
title: "List activities"
description: "Get the itemActivityOLDs from the activities navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List activities

Namespace: microsoft.graph

Get the itemActivityOLDs from the activities navigation property.

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
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/activities
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
If successful, this method returns a `200 OK` response code and a collection of [itemActivityOLD](../resources/itemactivityold.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_itemactivityold"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/activities
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemactivityold)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2677

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.itemActivityOLD",
      "id": "78232c74-2c74-7823-742c-2378742c2378",
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
        "lastRecordedDateTime": "2016-12-31T23:59:07.0452541+03:00",
        "observedDateTime": "2017-01-01T00:00:21.7260603+03:00",
        "recordedDateTime": "2017-01-01T00:02:58.0730674+03:00"
      }
    }
  ]
}
```

