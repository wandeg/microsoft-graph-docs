---
title: "Create teamsDeviceUsageUserCounts"
description: "Create a new teamsDeviceUsageUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create teamsDeviceUsageUserCounts

Create a new [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.teamsDeviceUsageUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the teamsDeviceUsageUserCounts object.

The following table shows the properties that are required when you create the teamsDeviceUsageUserCounts.

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
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamsdeviceusageusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.teamsDeviceUsageUserCounts not found
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageUserCounts",
  "reportRefreshDate": "Date",
  "web": 3,
  "windowsPhone": 12,
  "androidPhone": 12,
  "ios": 3,
  "mac": 3,
  "windows": 7,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsdeviceusageusercounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 318

{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageUserCounts",
  "id": "c6d25337-5337-c6d2-3753-d2c63753d2c6",
  "reportRefreshDate": "Date",
  "web": 3,
  "windowsPhone": 12,
  "androidPhone": 12,
  "ios": 3,
  "mac": 3,
  "windows": 7,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

