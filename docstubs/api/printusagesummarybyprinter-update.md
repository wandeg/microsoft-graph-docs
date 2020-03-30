---
title: "Update PrintUsageSummaryByPrinter"
description: "Update the properties of a PrintUsageSummaryByPrinter object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update PrintUsageSummaryByPrinter

Namespace: microsoft.graph

Update the properties of a [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object.

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
PATCH /reports/dailyPrintUsageSummariesByPrinter/{PrintUsageSummaryByPrinterId}
PATCH /reports/monthlyPrintUsageSummariesByPrinter/{PrintUsageSummaryByPrinterId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object.

The following table shows the properties that are required when you create the [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|printerId|String||
|usageDate|Date||
|completedBlackAndWhiteJobCount|Int64||
|completedColorJobCount|Int64||
|incompleteJobCount|Int64||



## Response
If successful, this method returns a `200 OK` response code and an updated [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_printusagesummarybyprinter"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/reports/dailyPrintUsageSummariesByPrinter/{PrintUsageSummaryByPrinterId}
Content-type: application/json
Content-length: 229

{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByPrinter",
  "printerId": "Printer Id value",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": 14,
  "completedColorJobCount": 6,
  "incompleteJobCount": 2
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
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByPrinter",
  "id": "8a28ddf7-ddf7-8a28-f7dd-288af7dd288a",
  "printerId": "Printer Id value",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": 14,
  "completedColorJobCount": 6,
  "incompleteJobCount": 2
}
```

