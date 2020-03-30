---
title: "getYammerDeviceUsageDistributionUserCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getYammerDeviceUsageDistributionUserCounts

Namespace: microsoft.graph



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
GET /reports/getYammerDeviceUsageDistributionUserCounts
GET /print/reports/{reportRootId}/getYammerDeviceUsageDistributionUserCounts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.yammerdeviceusagedistributionusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 381

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.yammerDeviceUsageDistributionUserCounts",
      "id": "e06d78a7-78a7-e06d-a778-6de0a7786de0",
      "reportRefreshDate": "Date",
      "web": 3,
      "windowsPhone": 12,
      "androidPhone": 12,
      "iPhone": 6,
      "iPad": 4,
      "other": 5,
      "reportPeriod": "Report Period value"
    }
  ]
}
```

