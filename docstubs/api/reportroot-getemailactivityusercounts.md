---
title: "getEmailActivityUserCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getEmailActivityUserCounts

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getEmailActivityUserCounts
GET /print/reports/{reportRootId}/getEmailActivityUserCounts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [emailActivitySummary](../resources/emailactivitysummary.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.emailactivitysummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.emailActivitySummary",
      "id": "557195d9-95d9-5571-d995-7155d9957155",
      "reportRefreshDate": "Date",
      "send": 4,
      "receive": 7,
      "read": 4,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

