---
title: "Get PrintUsageSummaryByPrinter"
description: "Read the properties and relationships of a PrintUsageSummaryByPrinter object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get PrintUsageSummaryByPrinter

Namespace: microsoft.graph

Read the properties and relationships of a [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageSummariesByPrinter/{PrintUsageSummaryByPrinterId}
GET /reports/monthlyPrintUsageSummariesByPrinter/{PrintUsageSummaryByPrinterId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_printusagesummarybyprinter"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/dailyPrintUsageSummariesByPrinter/{PrintUsageSummaryByPrinterId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.PrintUsageSummaryByPrinter"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.PrintUsageSummaryByPrinter",
    "id": "55f3bcf0-bcf0-55f3-f0bc-f355f0bcf355",
    "printerId": "String",
    "usageDate": "Date",
    "completedBlackAndWhiteJobCount": "Integer",
    "completedColorJobCount": "Integer",
    "incompleteJobCount": "Integer"
  }
}
```

