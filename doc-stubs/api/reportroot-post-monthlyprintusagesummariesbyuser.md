---
title: "Create monthlyPrintUsageSummariesByUser"
description: "Create a new monthlyPrintUsageSummariesByUser object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create monthlyPrintUsageSummariesByUser

Namespace: microsoft.graph

Create a new monthlyPrintUsageSummariesByUser object.

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
POST /reports/monthlyPrintUsageSummariesByUser
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object.

The following table shows the properties that are required when you create the [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userPrincipalName|String|**TODO: Add Description**|
|usageDate|Date|**TODO: Add Description**|
|completedBlackAndWhiteJobCount|Int64|**TODO: Add Description**|
|completedColorJobCount|Int64|**TODO: Add Description**|
|incompleteJobCount|Int64|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_printusagesummarybyuser_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/reports/monthlyPrintUsageSummariesByUser
Content-Type: application/json
Content-length: 247

{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByUser",
  "userPrincipalName": "String",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.printusagesummarybyuser"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByUser",
  "id": "e60429b4-29b4-e604-b429-04e6b42904e6",
  "userPrincipalName": "String",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer"
}
```

