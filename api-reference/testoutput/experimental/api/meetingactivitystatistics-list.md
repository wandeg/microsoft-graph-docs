---
title: "List meetingActivityStatisticses"
description: "List properties and relationships of the meetingActivityStatistics objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List meetingActivityStatisticses

List properties and relationships of the [meetingActivityStatistics](../resources/meetingactivitystatistics.md) objects.

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
GET ** Collection URI for microsoft.graph.meetingActivityStatistics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [meetingActivityStatistics](../resources/meetingactivitystatistics.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_meetingactivitystatistics"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.meetingActivityStatistics not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.meetingactivitystatistics)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 556

{
  "value": [
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
  ]
}
```

