---
title: "Get sharePointSiteUsageDetail"
description: "Read properties and relationships of the sharePointSiteUsageDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get sharePointSiteUsageDetail

Namespace: microsoft.graph

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
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.sharePointSiteUsageDetail not found
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
    "id": "6e05d61e-d61e-6e05-1ed6-056e1ed6056e",
    "reportRefreshDate": "Date",
    "siteId": "e6fd33e3-33e3-e6fd-e333-fde6e333fde6",
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

