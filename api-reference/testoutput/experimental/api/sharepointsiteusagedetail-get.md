---
title: "Get sharePointSiteUsageDetail"
description: "Read properties and relationships of the sharePointSiteUsageDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get sharePointSiteUsageDetail

Read properties and relationships of the [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Entity URI for microsoft.graph.sharePointSiteUsageDetail not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_sharepointsiteusagedetail"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.sharePointSiteUsageDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 706

{
  "value": {
    "@odata.type": "#microsoft.graph.sharePointSiteUsageDetail",
    "id": "cbf31882-1882-cbf3-8218-f3cb8218f3cb",
    "reportRefreshDate": "Date",
    "siteId": "005424d7-24d7-0054-d724-5400d7245400",
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
}
```

