---
title: "getOneDriveUsageAccountCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getOneDriveUsageAccountCounts

Namespace: microsoft.graph



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
GET /reports/getOneDriveUsageAccountCounts
GET /print/reports/{reportRootId}/getOneDriveUsageAccountCounts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onedriveusageaccountcounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.oneDriveUsageAccountCounts",
      "id": "f770c3d5-c3d5-f770-d5c3-70f7d5c370f7",
      "reportRefreshDate": "Date",
      "siteType": "Site Type value",
      "total": 5,
      "active": 6,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

