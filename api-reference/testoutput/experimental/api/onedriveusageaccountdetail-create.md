---
title: "Create oneDriveUsageAccountDetail"
description: "Create a new oneDriveUsageAccountDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create oneDriveUsageAccountDetail

Create a new [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) object.

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
POST ** Collection URI for microsoft.graph.oneDriveUsageAccountDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the oneDriveUsageAccountDetail object.

The following table shows the properties that are required when you create the oneDriveUsageAccountDetail.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|siteUrl|String||
|ownerDisplayName|String||
|ownerPrincipalName|String||
|isDeleted|Boolean||
|lastActivityDate|Date||
|fileCount|Int64||
|activeFileCount|Int64||
|storageUsedInBytes|Int64||
|storageAllocatedInBytes|Int64||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onedriveusageaccountdetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.oneDriveUsageAccountDetail not found
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.oneDriveUsageAccountDetail",
  "reportRefreshDate": "Date",
  "siteUrl": "https://example.com/siteUrl/",
  "ownerDisplayName": "Owner Display Name value",
  "ownerPrincipalName": "Owner Principal Name value",
  "isDeleted": true,
  "lastActivityDate": "Date",
  "fileCount": 9,
  "activeFileCount": 15,
  "storageUsedInBytes": 2,
  "storageAllocatedInBytes": 7,
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onedriveusageaccountdetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.oneDriveUsageAccountDetail",
  "id": "1e2f62b5-62b5-1e2f-b562-2f1eb5622f1e",
  "reportRefreshDate": "Date",
  "siteUrl": "https://example.com/siteUrl/",
  "ownerDisplayName": "Owner Display Name value",
  "ownerPrincipalName": "Owner Principal Name value",
  "isDeleted": true,
  "lastActivityDate": "Date",
  "fileCount": 9,
  "activeFileCount": 15,
  "storageUsedInBytes": 2,
  "storageAllocatedInBytes": 7,
  "reportPeriod": "Report Period value"
}
```

