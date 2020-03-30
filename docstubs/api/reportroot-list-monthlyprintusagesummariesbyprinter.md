---
title: "List monthlyPrintUsageSummariesByPrinter"
description: "Get the PrintUsageSummaryByPrinters from the monthlyPrintUsageSummariesByPrinter navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List monthlyPrintUsageSummariesByPrinter

Namespace: microsoft.graph

Get the PrintUsageSummaryByPrinters from the monthlyPrintUsageSummariesByPrinter navigation property.

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
GET /reports/monthlyPrintUsageSummariesByPrinter
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_printusagesummarybyprinter"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/monthlyPrintUsageSummariesByPrinter
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.printusagesummarybyprinter)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.PrintUsageSummaryByPrinter",
      "id": "0b5e21f5-21f5-0b5e-f521-5e0bf5215e0b",
      "printerId": "Printer Id value",
      "usageDate": "Date",
      "completedBlackAndWhiteJobCount": 14,
      "completedColorJobCount": 6,
      "incompleteJobCount": 2
    }
  ]
}
```

