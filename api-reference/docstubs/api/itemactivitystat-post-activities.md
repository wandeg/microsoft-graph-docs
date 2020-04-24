---
title: "Add activities"
description: "Add activities by posting to the activities collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add activities

Namespace: microsoft.graph

Add activities by posting to the activities collection.

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
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [itemActivity](../resources/itemactivity.md) object.

The following table shows the properties that are required when you create the [itemActivity](../resources/itemactivity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|access|[accessAction](../resources/accessaction.md)|**TODO: Add Description**|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|actor|[identitySet](../resources/identityset.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `204 No Content` response code and an [itemActivity](../resources/itemactivity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_itemactivity_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/$ref
Content-Type: application/json
Content-length: 550

{
  "@odata.type": "#microsoft.graph.itemActivity",
  "access": {
    "@odata.type": "microsoft.graph.accessAction"
  },
  "activityDateTime": "2017-01-01T00:03:07.3452024+03:00",
  "actor": {
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
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemactivity"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.itemActivity",
  "id": "a2210582-0582-a221-8205-21a2820521a2",
  "access": {
    "@odata.type": "microsoft.graph.accessAction"
  },
  "activityDateTime": "2017-01-01T00:03:07.3452024+03:00",
  "actor": {
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
  }
}
```

