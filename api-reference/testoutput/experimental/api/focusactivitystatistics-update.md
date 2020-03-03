---
title: "Update focusActivityStatistics"
description: "Update the properties of a focusActivityStatistics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update focusActivityStatistics

Namespace: microsoft.graph

Update the properties of a [focusActivityStatistics](../resources/focusactivitystatistics.md) object.

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
PATCH ** Entity URI for microsoft.graph.focusActivityStatistics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [focusActivityStatistics](../resources/focusactivitystatistics.md) object.

The following table shows the properties that are required when you create the [focusActivityStatistics](../resources/focusactivitystatistics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activitystatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|startDate|Date| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|duration|Duration| Inherited from [activityStatistics](../resources/activitystatistics.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [focusActivityStatistics](../resources/focusactivitystatistics.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_focusactivitystatistics"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.focusActivityStatistics not found
Content-type: application/json
Content-length: 214

{
  "@odata.type": "#microsoft.graph.focusActivityStatistics",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "-PT1M55.0810357S"
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
Content-Length: 263

{
  "@odata.type": "#microsoft.graph.focusActivityStatistics",
  "id": "6d401f1f-1f1f-6d40-1f1f-406d1f1f406d",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "-PT1M55.0810357S"
}
```

