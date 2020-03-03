---
title: "Update meetingActivityStatistics"
description: "Update the properties of a meetingActivityStatistics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update meetingActivityStatistics

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
In the request body, supply a JSON representation for the [meetingActivityStatistics](../resources/meetingActivityStatistics.md) object.

The following table shows the properties that are required when you create the [meetingActivityStatistics](../resources/meetingactivitystatistics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activityStatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|startDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|duration|Duration| Inherited from [activityStatistics](../resources/activityStatistics.md)|
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
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.meetingActivityStatistics not found
Content-type: application/json
Content-length: 422

{
  "@odata.type": "#microsoft.graph.meetingActivityStatistics",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "PT3M27.7161587S",
  "afterHours": "PT21.1795365S",
  "organized": "PT1M8.7021172S",
  "recurring": "-PT1M11.9254811S",
  "long": "PT38.7461735S",
  "conflicting": "PT3M34.2235549S",
  "multitasking": "PT2M11.8784902S"
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
Content-Length: 471

{
  "@odata.type": "#microsoft.graph.meetingActivityStatistics",
  "id": "8f4a6001-6001-8f4a-0160-4a8f01604a8f",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "PT3M27.7161587S",
  "afterHours": "PT21.1795365S",
  "organized": "PT1M8.7021172S",
  "recurring": "-PT1M11.9254811S",
  "long": "PT38.7461735S",
  "conflicting": "PT3M34.2235549S",
  "multitasking": "PT2M11.8784902S"
}
```

