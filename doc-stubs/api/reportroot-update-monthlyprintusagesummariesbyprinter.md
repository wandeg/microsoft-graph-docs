---
title: "Update monthlyPrintUsageSummariesByPrinter"
description: "Update the properties of a monthlyPrintUsageSummariesByPrinter object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update monthlyPrintUsageSummariesByPrinter

Namespace: microsoft.graph

Update the properties of a monthlyPrintUsageSummariesByPrinter object.

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
PATCH /reports/monthlyPrintUsageSummariesByPrinter
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object.

The following table shows the properties that are required when you create the [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|printerId|String|**TODO: Add Description**|
|usageDate|Date|**TODO: Add Description**|
|completedBlackAndWhiteJobCount|Int64|**TODO: Add Description**|
|completedColorJobCount|Int64|**TODO: Add Description**|
|incompleteJobCount|Int64|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_monthlyprintusagesummariesbyprinter"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/reports/monthlyPrintUsageSummariesByPrinter
Content-Type: application/json
Content-length: 242

{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByPrinter",
  "printerId": "String",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByPrinter",
  "id": "55f3bcf0-bcf0-55f3-f0bc-f355f0bcf355",
  "printerId": "String",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer"
}
```

