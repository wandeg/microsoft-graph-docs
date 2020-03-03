---
title: "List skypeForBusinessDeviceUsageDistributionUserCountses"
description: "List properties and relationships of the skypeForBusinessDeviceUsageDistributionUserCounts objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List skypeForBusinessDeviceUsageDistributionUserCountses

List properties and relationships of the [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) objects.

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
GET ** Collection URI for microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_skypeforbusinessdeviceusagedistributionusercounts"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.skypeforbusinessdeviceusagedistributionusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts",
      "id": "683f9284-9284-683f-8492-3f6884923f68",
      "reportRefreshDate": "Date",
      "windows": 7,
      "windowsPhone": 12,
      "androidPhone": 12,
      "iPhone": 6,
      "iPad": 4,
      "reportPeriod": "Report Period value"
    }
  ]
}
```

