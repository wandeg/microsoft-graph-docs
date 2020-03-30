---
title: "Update PrintUsageSummaryByUser"
description: "Update the properties of a PrintUsageSummaryByUser object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update PrintUsageSummaryByUser

Namespace: microsoft.graph

Update the properties of a [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object.

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
PATCH /reports/dailyPrintUsageSummariesByUser/{PrintUsageSummaryByUserId}
PATCH /reports/monthlyPrintUsageSummariesByUser/{PrintUsageSummaryByUserId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_printusagesummarybyuser"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/reports/dailyPrintUsageSummariesByUser/{PrintUsageSummaryByUserId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByUser",
  "id": "7a1a3a92-3a92-7a1a-923a-1a7a923a1a7a",
  "userPrincipalName": "User Principal Name value",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": 14,
  "completedColorJobCount": 6,
  "incompleteJobCount": 2
}
```

