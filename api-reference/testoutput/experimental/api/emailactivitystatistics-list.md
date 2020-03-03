---
title: "List emailActivityStatisticses"
description: "List properties and relationships of the emailActivityStatistics objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List emailActivityStatisticses

Namespace: microsoft.graph

List properties and relationships of the [emailActivityStatistics](../resources/emailactivitystatistics.md) objects.

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
GET ** Collection URI for microsoft.graph.emailActivityStatistics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [emailActivityStatistics](../resources/emailactivitystatistics.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_emailactivitystatistics"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.emailActivityStatistics not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.emailactivitystatistics)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 444

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.emailActivityStatistics",
      "id": "ed421464-1464-ed42-6414-42ed641442ed",
      "activity": "String",
      "startDate": "Date",
      "endDate": "Date",
      "timeZoneUsed": "Time Zone Used value",
      "duration": "-PT1M55.0810357S",
      "afterHours": "-PT1M34.3242013S",
      "readEmail": "-PT1M6.6321885S",
      "sentEmail": "-PT2M11.5873492S"
    }
  ]
}
```

