---
title: "reportRoot: getSharePointSiteUsageDetail"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getSharePointSiteUsageDetail

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /reports/getSharePointSiteUsageDetail
GET /print/reports/{reportRootId}/getSharePointSiteUsageDetail
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|period|String|**TODO: Add Description**|



## Response
If successful, this function returns a `200 OK` response code and a [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='parameterValue')
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sharepointsiteusagedetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharePointSiteUsageDetail",
      "id": "f45d528c-528c-f45d-8c52-5df48c525df4",
      "reportRefreshDate": "Date",
      "siteId": "f1b7bd04-bd04-f1b7-04bd-b7f104bdb7f1",
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

