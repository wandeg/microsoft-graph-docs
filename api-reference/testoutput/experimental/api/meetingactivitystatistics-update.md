---
title: "Update meetingActivityStatistics"
description: "Update the properties of a meetingActivityStatistics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update meetingActivityStatistics

Namespace: microsoft.graph

Update the properties of a [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object.

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
PATCH ** Entity URI for microsoft.graph.meetingActivityStatistics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object.

The following table shows the properties that are required when you create the [meetingActivityStatistics](../resources/meetingactivitystatistics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activitystatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|startDate|Date| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|duration|Duration| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|afterHours|Duration||
|organized|Duration||
|recurring|Duration||
|long|Duration||
|conflicting|Duration||
|multitasking|Duration||



## Response
If successful, this method returns a `200 OK` response code and an updated [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_meetingactivitystatistics"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.meetingActivityStatistics not found
Content-type: application/json
Content-length: 430

{
  "@odata.type": "#microsoft.graph.meetingActivityStatistics",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "-PT1M55.0810357S",
  "afterHours": "-PT1M34.3242013S",
  "organized": "-PT2M39.109661S",
  "recurring": "PT1M59.6924386S",
  "long": "-PT3M22.609558S",
  "conflicting": "-PT3M18.0945761S",
  "multitasking": "-PT1M33.7370046S"
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
Content-Length: 479

{
  "@odata.type": "#microsoft.graph.meetingActivityStatistics",
  "id": "2b96e2c8-e2c8-2b96-c8e2-962bc8e2962b",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "-PT1M55.0810357S",
  "afterHours": "-PT1M34.3242013S",
  "organized": "-PT2M39.109661S",
  "recurring": "PT1M59.6924386S",
  "long": "-PT3M22.609558S",
  "conflicting": "-PT3M18.0945761S",
  "multitasking": "-PT1M33.7370046S"
}
```

