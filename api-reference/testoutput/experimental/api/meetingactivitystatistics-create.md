---
title: "Create meetingActivityStatistics"
description: "Create a new meetingActivityStatistics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create meetingActivityStatistics

Create a new [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object.

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
POST ** Collection URI for microsoft.graph.meetingActivityStatistics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the meetingActivityStatistics object.

The following table shows the properties that are required when you create the meetingActivityStatistics.

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
If successful, this method returns a `201 Created` response code and a [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_meetingactivitystatistics_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.meetingActivityStatistics not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingactivitystatistics"
}
-->
``` http
HTTP/1.1 201 Created
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

