---
title: "Update itemActivityOLD"
description: "Update the properties of a itemActivityOLD object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update itemActivityOLD

Namespace: microsoft.graph

Update the properties of a [itemActivityOLD](../resources/itemactivityold.md) object.

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
PATCH /drives/{drivesId}/activities/{itemActivityOLDId}
PATCH /workbooks/{workbooksId}/activities/{itemActivityOLDId}
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}
PATCH /me/joinedGroups/{groupId}/drive/list/activities/{itemActivityOLDId}
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/activities/{itemActivityOLDId}
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/activities/{itemActivityOLDId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [itemActivityOLD](../resources/itemactivityold.md) object.

The following table shows the properties that are required when you create the [itemActivityOLD](../resources/itemactivityold.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|action|[itemActionSet](../resources/itemactionset.md)||
|actor|[identitySet](../resources/identityset.md)||
|times|[itemActivityTimeSet](../resources/itemactivitytimeset.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [itemActivityOLD](../resources/itemactivityold.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_itemactivityold"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/drives/{drivesId}/activities/{itemActivityOLDId}
Content-type: application/json
Content-length: 2271

{
  "@odata.type": "#microsoft.graph.itemActivityOLD",
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
    "lastRecordedDateTime": "2016-12-31T23:59:11.7173583+03:00",
    "observedDateTime": "2017-01-01T00:00:46.1782521+03:00",
    "recordedDateTime": "2016-12-31T23:57:24.9503923+03:00"
  }
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
Content-Length: 2320

{
  "@odata.type": "#microsoft.graph.itemActivityOLD",
  "id": "dc7452f1-52f1-dc74-f152-74dcf15274dc",
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
    "lastRecordedDateTime": "2016-12-31T23:59:11.7173583+03:00",
    "observedDateTime": "2017-01-01T00:00:46.1782521+03:00",
    "recordedDateTime": "2016-12-31T23:57:24.9503923+03:00"
  }
}
```

