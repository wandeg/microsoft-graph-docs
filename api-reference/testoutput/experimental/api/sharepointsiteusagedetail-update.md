---
title: "Update sharePointSiteUsageDetail"
description: "Update the properties of a sharePointSiteUsageDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update sharePointSiteUsageDetail

Update the properties of a [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.sharePointSiteUsageDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [sharePointSiteUsageDetail](../resources/sharePointSiteUsageDetail.md) object.

The following table shows the properties that are required when you create the [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|siteId|Guid||
|siteUrl|String||
|ownerDisplayName|String||
|ownerPrincipalName|String||
|isDeleted|Boolean||
|lastActivityDate|Date||
|fileCount|Int64||
|activeFileCount|Int64||
|pageViewCount|Int64||
|visitedPageCount|Int64||
|storageUsedInBytes|Int64||
|storageAllocatedInBytes|Int64||
|rootWebTemplate|String||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_sharepointsiteusagedetail"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.sharePointSiteUsageDetail not found
Content-type: application/json
Content-length: 604

{
  "@odata.type": "#microsoft.graph.sharePointSiteUsageDetail",
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
Content-Length: 653

{
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
```

