---
title: "Add monthlyPrintUsageSummariesByPrinter"
description: "Add monthlyPrintUsageSummariesByPrinter by posting to the monthlyPrintUsageSummariesByPrinter collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add monthlyPrintUsageSummariesByPrinter

Namespace: microsoft.graph

Add monthlyPrintUsageSummariesByPrinter by posting to the monthlyPrintUsageSummariesByPrinter collection.

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
POST /reports/monthlyPrintUsageSummariesByPrinter/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_printusagesummarybyprinter_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/reports/monthlyPrintUsageSummariesByPrinter
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
  "truncated": true,
  "@odata.type": "microsoft.graph.printusagesummarybyprinter"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByPrinter",
  "id": "d111ff4c-ff4c-d111-4cff-11d14cff11d1",
  "printerId": "Printer Id value",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": 14,
  "completedColorJobCount": 6,
  "incompleteJobCount": 2
}
```

