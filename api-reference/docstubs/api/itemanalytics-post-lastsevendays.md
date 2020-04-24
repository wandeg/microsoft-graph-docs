---
title: "Add lastSevenDays"
description: "Add lastSevenDays by posting to the lastSevenDays collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add lastSevenDays

Namespace: microsoft.graph

Add lastSevenDays by posting to the lastSevenDays collection.

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
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/lastSevenDays/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [itemActivityStat](../resources/itemactivitystat.md) object.

The following table shows the properties that are required when you create the [itemActivityStat](../resources/itemactivitystat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|access|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|create|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|delete|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|edit|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|move|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|isTrending|Boolean|**TODO: Add Description**|
|incompleteData|[incompleteData](../resources/incompletedata.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `204 No Content` response code and an [itemActivityStat](../resources/itemactivitystat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_itemactivitystat_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/lastSevenDays/$ref
Content-Type: application/json
Content-length: 786

{
  "@odata.type": "#microsoft.graph.itemActivityStat",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
  "access": {
    "@odata.type": "microsoft.graph.itemActionStat",
    "actionCount": 11,
    "actorCount": 10
  },
  "create": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "delete": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "edit": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "move": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "isTrending": true,
  "incompleteData": {
    "@odata.type": "microsoft.graph.incompleteData",
    "missingDataBeforeDateTime": "2017-01-01T00:00:00.6050594+03:00",
    "wasThrottled": true
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemactivitystat"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.itemActivityStat",
  "id": "0328aa2e-aa2e-0328-2eaa-28032eaa2803",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
  "access": {
    "@odata.type": "microsoft.graph.itemActionStat",
    "actionCount": 11,
    "actorCount": 10
  },
  "create": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "delete": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "edit": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "move": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "isTrending": true,
  "incompleteData": {
    "@odata.type": "microsoft.graph.incompleteData",
    "missingDataBeforeDateTime": "2017-01-01T00:00:00.6050594+03:00",
    "wasThrottled": true
  }
}
```

