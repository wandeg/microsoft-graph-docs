---
title: "getSharePointSiteUsageDetail"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getSharePointSiteUsageDetail

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
GET /reports/getSharePointSiteUsageDetail
GET /print/reports/{reportRootId}/getSharePointSiteUsageDetail
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
If successful, this function returns a `200 OK` response code and a [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sharepointsiteusagedetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 754

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharePointSiteUsageDetail",
      "id": "56a5d608-d608-56a5-08d6-a55608d6a556",
      "reportRefreshDate": "Date",
      "siteId": "003ad312-d312-003a-12d3-3a0012d33a00",
      "siteUrl": "https://example.com/siteUrl/",
      "ownerDisplayName": "Owner Display Name value",
      "ownerPrincipalName": "Owner Principal Name value",
      "isDeleted": true,
      "lastActivityDate": "Date",
      "fileCount": 9,
      "activeFileCount": 15,
      "pageViewCount": 13,
      "visitedPageCount": 0,
      "storageUsedInBytes": 2,
      "storageAllocatedInBytes": 7,
      "rootWebTemplate": "Root Web Template value",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

