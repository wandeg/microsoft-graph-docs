---
title: "Get PrintUsageSummaryByUser"
description: "Read properties and relationships of the PrintUsageSummaryByUser object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get PrintUsageSummaryByUser

Namespace: microsoft.graph

Read properties and relationships of the [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object.

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
GET /reports/dailyPrintUsageSummariesByUser/{PrintUsageSummaryByUserId}
GET /reports/monthlyPrintUsageSummariesByUser/{PrintUsageSummaryByUserId}
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
If successful, this method returns a `200 OK` response code and [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_printusagesummarybyuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/dailyPrintUsageSummariesByUser/{PrintUsageSummaryByUserId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.PrintUsageSummaryByUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 325

{
  "value": {
    "@odata.type": "#microsoft.graph.PrintUsageSummaryByUser",
    "id": "e5e9096a-096a-e5e9-6a09-e9e56a09e9e5",
    "userPrincipalName": "User Principal Name value",
    "usageDate": "Date",
    "completedBlackAndWhiteJobCount": 14,
    "completedColorJobCount": 6,
    "incompleteJobCount": 2
  }
}
```

