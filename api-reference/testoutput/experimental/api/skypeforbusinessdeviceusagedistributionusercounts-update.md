---
title: "Update skypeForBusinessDeviceUsageDistributionUserCounts"
description: "Update the properties of a skypeForBusinessDeviceUsageDistributionUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update skypeForBusinessDeviceUsageDistributionUserCounts

Update the properties of a [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeForBusinessDeviceUsageDistributionUserCounts.md) object.

The following table shows the properties that are required when you create the [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|windows|Int32||
|windowsPhone|Int32||
|androidPhone|Int32||
|iPhone|Int32||
|iPad|Int32||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_skypeforbusinessdeviceusagedistributionusercounts"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts not found
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts",
  "reportRefreshDate": "Date",
  "windows": 7,
  "windowsPhone": 12,
  "androidPhone": 12,
  "iPhone": 6,
  "iPad": 4,
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

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
```

