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

## HTTP Request
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
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [activityStatistics](../resources/activitystatistics.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}
-->
``` http
GET https://graph.microsoft.com/localtest/activitystatistics/{activitystatisticsId}
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
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.activityStatistics",
    "id": "53e767f4-67f4-53e7-f467-e753f467e753",
    "activity": "String",
    "startDate": "Date",
    "endDate": "Date",
    "timeZoneUsed": "Time Zone Used value",
    "duration": "-PT1M55.0810357S"
  }
}
```

