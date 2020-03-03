---
title: "Create yammerDeviceUsageUserCounts"
description: "Create a new yammerDeviceUsageUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create yammerDeviceUsageUserCounts

Create a new [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.yammerDeviceUsageUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the yammerDeviceUsageUserCounts object.

The following table shows the properties that are required when you create the yammerDeviceUsageUserCounts.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|web|Int32||
|windowsPhone|Int32||
|androidPhone|Int32||
|iPhone|Int32||
|iPad|Int32||
|other|Int32||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_yammerdeviceusageusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.yammerDeviceUsageUserCounts not found
Content-type: application/json
Content-length: 272

{
  "@odata.type": "#microsoft.graph.yammerDeviceUsageUserCounts",
  "reportRefreshDate": "Date",
  "web": 3,
  "windowsPhone": 12,
  "androidPhone": 12,
  "iPhone": 6,
  "iPad": 4,
  "other": 5,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerdeviceusageusercounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 321

{
  "@odata.type": "#microsoft.graph.yammerDeviceUsageUserCounts",
  "id": "dc169f2b-9f2b-dc16-2b9f-16dc2b9f16dc",
  "reportRefreshDate": "Date",
  "web": 3,
  "windowsPhone": 12,
  "androidPhone": 12,
  "iPhone": 6,
  "iPad": 4,
  "other": 5,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

