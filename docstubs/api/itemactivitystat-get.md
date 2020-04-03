---
title: "Get itemActivityStat"
description: "Read properties and relationships of the itemActivityStat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get itemActivityStat

Namespace: microsoft.graph

Read properties and relationships of the [itemActivityStat](../resources/itemactivitystat.md) object.

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
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}
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
If successful, this method returns a `200 OK` response code and [itemActivityStat](../resources/itemactivitystat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_itemactivitystat"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemActivityStat"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 908

{
  "value": {
    "@odata.type": "#microsoft.graph.itemActivityStat",
    "id": "b3bdfd6c-fd6c-b3bd-6cfd-bdb36cfdbdb3",
    "startDateTime": "2016-12-31T23:59:00.3105042+00:00",
    "endDateTime": "2016-12-31T23:57:26.2105705+00:00",
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
      "missingDataBeforeDateTime": "2016-12-31T23:57:30.3813273+00:00",
      "wasThrottled": true
    }
  }
}
```

