---
title: "Get activityStatistics"
description: "Read properties and relationships of the activityStatistics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get activityStatistics

Namespace: microsoft.graph

Read properties and relationships of the [activityStatistics](../resources/activitystatistics.md) object.

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
GET /activitystatistics/{activitystatisticsId}
GET /me/analytics/activityStatistics/{activityStatisticsId}
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
If successful, this method returns a `200 OK` response code and [activityStatistics](../resources/activitystatistics.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}
-->
``` http
GET https://graph.microsoft.com/beta/activitystatistics/{activitystatisticsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityStatistics"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "value": {
    "@odata.type": "#microsoft.graph.activityStatistics",
    "id": "786ebe3d-be3d-786e-3dbe-6e783dbe6e78",
    "activity": "String",
    "startDate": "Date",
    "endDate": "Date",
    "timeZoneUsed": "Time Zone Used value",
    "duration": "PT58.0389239S"
  }
}
```

