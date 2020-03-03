---
title: "List focusActivityStatisticses"
description: "List properties and relationships of the focusActivityStatistics objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List focusActivityStatisticses

List properties and relationships of the [focusActivityStatistics](../resources/focusactivitystatistics.md) objects.

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
GET ** Collection URI for microsoft.graph.focusActivityStatistics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [focusActivityStatistics](../resources/focusactivitystatistics.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_focusactivitystatistics"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.focusActivityStatistics not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.focusactivitystatistics)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 323

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.focusActivityStatistics",
      "id": "f835d8b2-d8b2-f835-b2d8-35f8b2d835f8",
      "activity": "String",
      "startDate": "Date",
      "endDate": "Date",
      "timeZoneUsed": "Time Zone Used value",
      "duration": "PT3M27.7161587S"
    }
  ]
}
```

