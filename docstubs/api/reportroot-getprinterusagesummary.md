---
title: "getPrinterUsageSummary"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getPrinterUsageSummary

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
GET /print/reports/getPrinterUsageSummary
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
|printerId|String||
|periodStart|DateTimeOffset||
|periodEnd|DateTimeOffset||



## Response
If successful, this function returns a `200 OK` response code and a [printerUsageSummary](../resources/printerusagesummary.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getprinterusagesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/reports/getPrinterUsageSummary(printerId='parameterValue',periodStart=1/1/2017 12:00:52 AM +00:00,periodEnd=12/31/2016 11:58:26 PM +00:00)
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerusagesummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 81

{
  "value": {
    "@odata.type": "microsoft.graph.printerUsageSummary"
  }
}
```

