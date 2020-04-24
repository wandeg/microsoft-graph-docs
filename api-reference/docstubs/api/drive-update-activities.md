---
title: "Update activities"
description: "Update the properties of an activities object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update activities

Namespace: microsoft.graph

Update the properties of an activities object.

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
PATCH /drive/activities
PATCH /drives/{drivesId}/activities
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [itemActivityOLD](../resources/itemactivityold.md) object.

The following table shows the properties that are required when you create the [itemActivityOLD](../resources/itemactivityold.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|action|[itemActionSet](../resources/itemactionset.md)|**TODO: Add Description**|
|actor|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|times|[itemActivityTimeSet](../resources/itemactivitytimeset.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [itemActivityOLD](../resources/itemactivityold.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_activities"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/drive/activities
Content-Type: application/json
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
    "lastRecordedDateTime": "2016-12-31T23:58:05.7284026+03:00",
    "observedDateTime": "2017-01-01T00:03:30.6225791+03:00",
    "recordedDateTime": "2016-12-31T23:56:35.2919298+03:00"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.itemActivityOLD",
  "id": "98f47719-7719-98f4-1977-f4981977f498",
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
    "lastRecordedDateTime": "2016-12-31T23:58:05.7284026+03:00",
    "observedDateTime": "2017-01-01T00:03:30.6225791+03:00",
    "recordedDateTime": "2016-12-31T23:56:35.2919298+03:00"
  }
}
```

