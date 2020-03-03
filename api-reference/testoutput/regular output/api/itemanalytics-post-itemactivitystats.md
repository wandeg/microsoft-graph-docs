---
title: "Add itemActivityStats"
description: "Add itemActivityStats by posting to the itemActivityStats collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add itemActivityStats

Add itemActivityStats by posting to the itemActivityStats collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/drive/items/{driveItemId}/analytics/itemActivityStats/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the itemActivityStat object.

The following table shows the properties that are required when you create the itemActivityStat.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|access|[itemActionStat](../resources/itemActionStat.md)||
|create|[itemActionStat](../resources/itemActionStat.md)||
|delete|[itemActionStat](../resources/itemActionStat.md)||
|edit|[itemActionStat](../resources/itemActionStat.md)||
|move|[itemActionStat](../resources/itemActionStat.md)||
|isTrending|Boolean||
|incompleteData|[incompleteData](../resources/incompleteData.md)||



## Response
If successful, this method returns a `201 Created` response code and a [itemActivityStat](../resources/itemactivitystat.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_itemactivitystat_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/drive/items/{driveItemId}/analytics/itemActivityStats
Content-type: application/json
Content-length: 786

{
  "@odata.type": "#microsoft.graph.itemActivityStat",
  "startDateTime": "2017-01-01T00:02:52.8537882+03:00",
  "endDateTime": "2017-01-01T00:00:48.5623528+03:00",
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
    "missingDataBeforeDateTime": "2016-12-31T23:58:26.7841266+03:00",
    "wasThrottled": true
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemactivitystat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 835

{
  "@odata.type": "#microsoft.graph.itemActivityStat",
  "id": "c4dfb8eb-b8eb-c4df-ebb8-dfc4ebb8dfc4",
  "startDateTime": "2017-01-01T00:02:52.8537882+03:00",
  "endDateTime": "2017-01-01T00:00:48.5623528+03:00",
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
    "missingDataBeforeDateTime": "2016-12-31T23:58:26.7841266+03:00",
    "wasThrottled": true
  }
}
```

