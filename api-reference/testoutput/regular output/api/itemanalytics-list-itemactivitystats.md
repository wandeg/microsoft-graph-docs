---
title: "List itemActivityStats"
description: "Get the itemActivityStats from the itemActivityStats navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List itemActivityStats

Get the itemActivityStats from the itemActivityStats navigation property.

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
GET /me/drive/items/{driveItemId}/analytics/itemActivityStats
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [itemActivityStat](../resources/itemactivitystat.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_itemactivitystat"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/me/drive/items/{driveItemId}/analytics/itemActivityStats
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemactivitystat)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 976

{
  "value": [
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
  ]
}
```

