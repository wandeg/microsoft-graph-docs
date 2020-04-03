---
title: "Add dailyPrintUsageSummariesByUser"
description: "Add dailyPrintUsageSummariesByUser by posting to the dailyPrintUsageSummariesByUser collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add dailyPrintUsageSummariesByUser

Namespace: microsoft.graph

Add dailyPrintUsageSummariesByUser by posting to the dailyPrintUsageSummariesByUser collection.

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
POST /reports/dailyPrintUsageSummariesByUser/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object.

The following table shows the properties that are required when you create the [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userPrincipalName|String||
|usageDate|Date||
|completedBlackAndWhiteJobCount|Int64||
|completedColorJobCount|Int64||
|incompleteJobCount|Int64||



## Response
If successful, this method returns a `201 Created` response code and a [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_printusagesummarybyuser_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/reports/dailyPrintUsageSummariesByUser
Content-type: application/json
Content-length: 243

{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByUser",
  "userPrincipalName": "User Principal Name value",
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
  "@odata.type": "microsoft.graph.printusagesummarybyuser"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByUser",
  "id": "88996855-6855-8899-5568-998855689988",
  "userPrincipalName": "User Principal Name value",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": 14,
  "completedColorJobCount": 6,
  "incompleteJobCount": 2
}
```

