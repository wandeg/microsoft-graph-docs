---
title: "reportRoot: getPrintUsageSummariesByTimeSpan"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getPrintUsageSummariesByTimeSpan

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
GET /print/reports/getPrintUsageSummariesByTimeSpan
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
|periodStart|DateTimeOffset||
|periodEnd|DateTimeOffset||
|timeSpanInMinutes|Int32||



## Response
If successful, this function returns a `200 OK` response code and a [printUsageSummary](../resources/printusagesummary.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getprintusagesummariesbytimespan"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/reports/getPrintUsageSummariesByTimeSpan(periodStart=1/1/2017 12:01:48 AM +00:00,periodEnd=12/31/2016 11:59:18 PM +00:00,timeSpanInMinutes=1)
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.printusagesummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "value": [
    {
      "@odata.type": "microsoft.graph.printUsageSummary"
    }
  ]
}
```

