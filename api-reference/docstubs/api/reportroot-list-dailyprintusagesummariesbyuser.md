---
title: "List dailyPrintUsageSummariesByUser"
description: "Get the PrintUsageSummaryByUsers from the dailyPrintUsageSummariesByUser navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List dailyPrintUsageSummariesByUser

Namespace: microsoft.graph

Get the PrintUsageSummaryByUsers from the dailyPrintUsageSummariesByUser navigation property.

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
GET /reports/dailyPrintUsageSummariesByUser
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
If successful, this method returns a `200 OK` response code and a collection of [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_printusagesummarybyuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/dailyPrintUsageSummariesByUser
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.printusagesummarybyuser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 353

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.PrintUsageSummaryByUser",
      "id": "2c53c5be-c5be-2c53-bec5-532cbec5532c",
      "userPrincipalName": "User Principal Name value",
      "usageDate": "Date",
      "completedBlackAndWhiteJobCount": 14,
      "completedColorJobCount": 6,
      "incompleteJobCount": 2
    }
  ]
}
```

