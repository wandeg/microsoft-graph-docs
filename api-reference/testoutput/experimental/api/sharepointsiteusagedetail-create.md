---
title: "Create sharePointSiteUsageDetail"
description: "Create a new sharePointSiteUsageDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create sharePointSiteUsageDetail

Create a new [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) object.

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
POST ** Collection URI for microsoft.graph.sharePointSiteUsageDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the sharePointSiteUsageDetail object.

The following table shows the properties that are required when you create the sharePointSiteUsageDetail.

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
If successful, this method returns a `201 Created` response code and a [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_sharepointsiteusagedetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.sharePointSiteUsageDetail not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.sharepointsiteusagedetail"
}
-->
``` http
HTTP/1.1 201 Created
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

