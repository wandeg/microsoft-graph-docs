---
title: "Create itemActivityStat"
description: "Create a new itemActivityStat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create itemActivityStat

Namespace: microsoft.graph

Create a new [itemActivityStat](../resources/itemactivitystat.md) object.

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
POST /me/drive/items/{driveItemId}/analytics/itemActivityStats
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [itemActivityStat](../resources/itemactivitystat.md) object.

The following table shows the properties that are required when you create the [itemActivityStat](../resources/itemactivitystat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|access|[itemActionStat](../resources/itemactionstat.md)||
|create|[itemActionStat](../resources/itemactionstat.md)||
|delete|[itemActionStat](../resources/itemactionstat.md)||
|edit|[itemActionStat](../resources/itemactionstat.md)||
|move|[itemActionStat](../resources/itemactionstat.md)||
|isTrending|Boolean||
|incompleteData|[incompleteData](../resources/incompletedata.md)||



## Response
If successful, this method returns a `201 Created` response code and a [itemActivityStat](../resources/itemactivitystat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_itemactivitystat_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/analytics/itemActivityStats
Content-type: application/json
Content-length: 786

{
  "@odata.type": "#microsoft.graph.itemActivityStat",
  "startDateTime": "2017-01-01T00:00:26.7994828+03:00",
  "endDateTime": "2016-12-31T23:57:36.1520435+03:00",
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
    "missingDataBeforeDateTime": "2017-01-01T00:00:17.2858665+03:00",
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
  "id": "01b4bc2f-bc2f-01b4-2fbc-b4012fbcb401",
  "startDateTime": "2017-01-01T00:00:26.7994828+03:00",
  "endDateTime": "2016-12-31T23:57:36.1520435+03:00",
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
    "missingDataBeforeDateTime": "2017-01-01T00:00:17.2858665+03:00",
    "wasThrottled": true
  }
}
```

