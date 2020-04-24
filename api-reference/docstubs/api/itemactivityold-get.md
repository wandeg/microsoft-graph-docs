---
title: "Get itemActivityOLD"
description: "Read the properties and relationships of an itemActivityOLD object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get itemActivityOLD

Namespace: microsoft.graph

Read the properties and relationships of an [itemActivityOLD](../resources/itemactivityold.md) object.

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
**Note:** The response object shown here might be shortened for readability.
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
}
```

