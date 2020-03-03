---
title: "Create teamsDeviceUsageDistributionUserCounts"
description: "Create a new teamsDeviceUsageDistributionUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create teamsDeviceUsageDistributionUserCounts

Namespace: microsoft.graph

Create a new [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.teamsDeviceUsageDistributionUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) object.

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
If successful, this method returns a `201 Created` response code and a [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamsdeviceusagedistributionusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.teamsDeviceUsageDistributionUserCounts not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsdeviceusagedistributionusercounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 305

{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageDistributionUserCounts",
  "id": "caf953a1-53a1-caf9-a153-f9caa153f9ca",
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

