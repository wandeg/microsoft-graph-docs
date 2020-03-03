---
title: "Update teamsDeviceUsageDistributionUserCounts"
description: "Update the properties of a teamsDeviceUsageDistributionUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsDeviceUsageDistributionUserCounts

Update the properties of a [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.teamsDeviceUsageDistributionUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [teamsDeviceUsageDistributionUserCounts](../resources/teamsDeviceUsageDistributionUserCounts.md) object.

The following table shows the properties that are required when you create the [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|web|Int64||
|windowsPhone|Int64||
|androidPhone|Int64||
|ios|Int64||
|mac|Int64||
|windows|Int64||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamsdeviceusagedistributionusercounts"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.teamsDeviceUsageDistributionUserCounts not found
Content-type: application/json
Content-length: 256

{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageDistributionUserCounts",
  "reportRefreshDate": "Date",
  "web": 3,
  "windowsPhone": 12,
  "androidPhone": 12,
  "ios": 3,
  "mac": 3,
  "windows": 7,
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
Content-Length: 305

{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageDistributionUserCounts",
  "id": "b3c4ab5b-ab5b-b3c4-5bab-c4b35babc4b3",
  "reportRefreshDate": "Date",
  "web": 3,
  "windowsPhone": 12,
  "androidPhone": 12,
  "ios": 3,
  "mac": 3,
  "windows": 7,
  "reportPeriod": "Report Period value"
}
```

